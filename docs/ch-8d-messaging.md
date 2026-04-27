---
title: 8d. Clinical Messaging
---

# 8d. Clinical Messaging

### 8d.1 Introduction

This chapter will deal with the clinical communications supporting
day-to-day patient care, which involve the sending of data to and from
GP systems.

An important part of the safe and effective use of clinical data
received from elsewhere is to have an appreciation of the limitations
such data may have, as a consequence of the methods of their capture in
a remote system, and their subsequent transformation, transfer to and
incorporation into the GP system. Mention will therefore be made of
'health warnings' practitioners should bear in mind, when using data
originated elsewhere.

Where, as is nowadays the case, diverse mechanisms are emerging to
support a particular business flow of information, guidance will be
offered on the system-independent processes needed to handle such data
and information transfers.

### 8d.2 Background

The messaging discussed here is the transfer of clinical data between
computer systems, the data being structured (organised, coded in whole
or in part, and assembled) to a standard observed by both systems. This
structuring means that the receiver can 'understand' all or part of the
data's meaning - as if they had been natively entered.

Every practitioner will be acquainted with the laboratory investigation
reports, standards for which were developed in 1993-5 and which now have
near-universal implementation after the Pathology Messaging
Implementation Project (PMIP). GP2GP record transfer and then GP Summary
Care Record uploads (see chapters 8b & 8e respectively) are the next
most widely-used messaging applications. Other clinical messaging,
though now on the threshold of a major expansion, has been slow to
develop.

Currently, all new messaging travels via the NHS Spine, for which
accreditation to the demographic and other services is needed -- but is
not in place for many Trust systems. So the recent work to develop the
NHS Interoperability Toolkit[^1] (NHS ITK -- sets standards based on web
services for (any) systems to transmit data securely between themselves)
will make communication between GP and Trust systems easier to
establish, and through lowering the barriers to entry, will involve more
systems as participants to the communications.

This diversity in messaging, allied to the increasing number of
intermediate solutions being offered by document transfer systems (vide
infra) and to the possibilities of remote login to Trust systems, brings
both opportunity and threat. With the opportunity to participate in a
communication that has long been desired (e.g. inpatient discharge
summary) comes the threat of confusion from a variety of means of
implementing it.

The electronic transfer of documents (by NHSmail or by other means) and
the transfer of data through web services has become sufficiently
sophisticated that a clinician may not readily appreciate whether the
data and text he or she is looking at is in the local or in a remote
computer system, and is, or is not discoverable by a search of his/her
system. This is likely not to matter for the immediate needs of the
patient, but the clinician's responsibility for keeping adequate records
does have implications for whether he/she: makes a local entry of data
from a remote system that has been used for decision making; or makes a
coded entry to allow later retrieval of data imported as text. It is
particularly important to ensure that, when a patient record is
transferred to a new general practice, information that is held on a
remote system is not lost as a result.

### 8d.2.1 From this background, some guidance can be offered

-   *Clinicians have a responsibility to be trained in and to understand
    in broad terms the limitations of the clinical communication tools
    they use.*

-   *For each new clinical messaging or communication facility offered
    to them, clinicians should ask some questions of the supplier,
    taking advice if necessary from their local support and through them
    from NHS CfH:*

    -   *To what extent are data and information I am receiving to be
        incorporated into the local medical record and discoverable by
        searches on my system?*

    -   *To what extent and in what form (coded or text) will data I am
        receiving be subsequently exported to the patient's next GP by a
        GP2GP record transfer?*

    -   *For data which passes out of my clinical system, to whom will
        it go and what will it be used for?*

    -   *Which are the standards governing the transfer, and are these
        all open or are any proprietary?*

    -   *Does the transfer conform to NHS guidance on encryption &
        security*[^2]*?*

    -   *Has the NHS CfH clinical safety process been used to assure
        this development, and if not, what stands in its place?*

    -   *What training am I and any of my staff who are to use this
        software going to receive?*

### 8d.3 Processes involved in handling clinical messaging data transfers

This section concentrates on incoming data handling. Outgoing data by
messaging is less demanding, is covered by guidance above, and (apart
from ETP, SCR and GP2GP) there are no applications in immediate
prospect.

All the incoming messaging applications to be discussed specifically
below (Pathology, Radiology, OOH encounter, A/E or OPD attendance and
I/P discharge) have common characteristics in the way they need to be
handled -- some preparatory work needs to be done to confirm validity
and to deliver them to the right person and they then need to be
processed by a clinician and filed or archived away. The main steps in
this might be summarised;

-   *An administrative process deals with corrupted or missing
    transmissions*

-   *An administrative process matches manually those patients or
    clinicians identified in the message for whom an adequate machine
    match is not possible*

-   *An administrative process assigns or reassigns messages to the
    work-stream for the clinician who is to attend to them*

-   *A clinical process of examining and acting on the contents on the
    message occurs; this may involve coding or re-coding some of the
    message content*

-   *An administrative process of filing the message content into the
    clinical record and clearing it from the work-stream occurs. This is
    often triggered by the clinician*

A large number of diverse communications converge on every practising
clinician and these are gradually moving to be presented through the
medium of the clinical records system. There is clear potential for
failure if the handling mechanisms do not offer maximum utility and
efficiency, and this is a prospective systems design issue.

Based upon this, some guidance can be offered:

-   *For every clinical communication stream, practices should appoint
    and train one or more members of staff (and at least one deputy to
    cover for sickness/leave) who is responsible for the administrative
    processes outlined above*

-   *Practices should have a protocol for handling laboratory results
    and other clinical messages which are intended for a clinician's
    attention but which arrive during his or her absence*

### 8d.4 Pathology

The PMIP messages in widespread use were scoped for use for Haematology,
Biochemistry and Microbiology reports, and because of their success in
this and the lack of development of other clinical messaging vehicles,
they have since been used for wider purposes, including for cytology and
radiology reports.

In 2005-6 new pathology messages were developed by NHS CfH[^3] to extend
the scope of use to requesting and the full range of report disciplines
and, supported by the Carter Report into Pathology[^4], they await a
political impetus for implementation. A current NHS CfH project[^5] is
using the new report message to pilot the transmission of neonatal Blood
Spot testing results in to departments of Child Health.

PMIP messages usually identify the investigations conducted by Read
codes but also permit un-coded investigations. Systems have offered
facilities to allow practices to encode these tests but this is to be
deprecated because of the risk of not doing this as the laboratory
would, had it been faced with the same code-list choices. This would not
only have the potential to cause a later misapprehension, but also, in
the age of GP2GP transfers, could cause tests not to be recognised as
equivalent in the destination GP system.

As a result of the historical independence of pathology laboratories,
there are many labs which are conducting the same investigations, and
reporting them using different units of measurement. Examples include
the measurement of Haemoglobin concentration expressed in grammes per
decilitre and grammes per litre. An initiative from within the
Pathology[^6] community is working to reduce these non-uniformities, but
it will take many years before this is complete. Meantime, GP2GP record
transfers and centrally-hosted GP systems with insufficient defences
against these differences risk mixing these non-comparable data and
leading to clinician confusion.

Based upon this, the following guidance may be offered;

-   *Practices and laboratories using PMIP report messages should avail
    themselves of the extensive implementation advice*[^7] *available*

-   *Practices should encourage their laboratories to use the National
    Message Assurance Service (NMAS*[^8]*) for periodic checking of
    their message output and where problems arise in use*

-   *Practices should be aware that where laboratory tests are not
    identified by Read codes, they will not be discovered by subsequent
    searches*

-   *Practices should encourage their laboratories to use valid Read
    codes for identifying investigations, and where such codes do not
    exist, to apply for their inclusion in the Bounded Codelist*[^9]
    *that constrains use of the PMIP messages and in the new National
    Catalogue for Laboratory Medicine*[^10]

-   *Practices should exercise great caution in using facilities which
    may be provided to map uncoded investigations in laboratory reports
    to Read codes: it is in every way preferable for the laboratories
    themselves to do this mapping and to involve them in the problem*

-   *Practices should be aware of the limitations in aggregating report
    data (say into trend lines) caused by the changing of: codes used to
    identify investigations; of laboratory methods; and of laboratory
    reference ranges*

-   *Practices should be aware that the import of laboratory results
    from a patient's previous practice via GP2GP transfer may bring
    together instances of the same investigation carried out in
    different laboratories, using different methods and reported using
    different units of measurement*

### 8d.5 Radiology

As has been mentioned earlier, the PMIP report messages are being used
in a number of places to convey reports for radiology, a subset of
Diagnostic Imaging (DI) modalities. New HL7v3 radiology request and
report message standards have been developed in NHS CfH. As yet, there
are no smartcard-enabled PACS/RIS (radiology) systems, and until this is
the case, these messages will not be able to travel via the spine to
GPs. However the NHS ITK mentioned earlier offers hope of an earlier
step towards using these messages.

### 8d.6 Out Of Hours (OOH)

The dominant supplier for OOH centres (Adastra) offers an electronic
document transfer of details of an OOH encounter and there is widespread
use of this. It is text-based and so practices will need to make their
own decisions and to personally encode them if they wish to store
clinically-coded information relating to these.

Arising from this, guidance can be offered;

-   *Practices receiving messages about OOH encounters should make
    decisions on clinical coding just as they would had the
    communication been received on paper*

### 8d.7 A/E encounter, outpatients encounter, inpatients discharge.

These three communications are grouped together because they share
similar characteristics. Messages developed by NHS CfH are not now
planned to be implemented as part of a future development of the Summary
Care Record. The path to developing the capability of GP systems to
receive them is reasonably clear, the capacity of Trust systems to send
them seems further off.

Meantime, a wide variety of initiatives is giving GPs access to some of
this information in varying degrees of structure, ranging from
structured messages based upon a project in 2006 in Kettering, to
unstructured document transfer (e.g. into the Docman add-on). In this
environment, the precautions advised of practices in section 8d.2 and
8d.6 are also applicable.

[^1]: <http://www.connectingforhealth.nhs.uk/systemsandservices/interop>

[^2]: <http://www.connectingforhealth.nhs.uk/systemsandservices/infogov/security>

[^3]: [http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/modernising/projects/gp](%20http:/www.connectingforhealth.nhs.uk/systemsandservices/pathology/modernising/projects/gp)

[^4]: <http://webarchive.nationalarchives.gov.uk/+/www.dh.gov.uk/en/Healthcare/Pathology/DH_075531>

[^5]: <http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/modernising/projects/newborn>

[^6]: <http://www.pathologyharmony.co.uk/>

[^7]: <http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/edifact/pmip/guidance>

[^8]: <http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/edifact/nmas>

[^9]: <http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/edifact/technical/standards/bounded>

[^10]: <http://www.connectingforhealth.nhs.uk/systemsandservices/pathology/modernising/projects/nlmc>
