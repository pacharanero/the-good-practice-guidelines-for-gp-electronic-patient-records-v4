---
title: 8e. The Summary Care Record and the Emergency Care Summary
---

# 8e. The Summary Care Record and the Emergency Care Summary

### 8e.1 Introduction {#e.1-introduction .ListParagraph}

The Summary Care Record (SCR)[^1] in England and the Emergency Care
Summary (ECS)[^2] in Scotland are resources designed to assist in the
management of patients in urgent and emergency care settings
(OOH/NHS24/A+E etc). Each resource is populated by selective extracts
from the GP record. In both cases, the core extract consists of all
current repeat medication and all allergies/adverse reactions identified
in the source record. The SCR also includes recently discontinued repeat
medication and any acute medication issued in the previous six months.

The SCR is capable of being added to with more coded data and associated
free text, subject to the decisions of the patient and responsible
clinician.

The ECS does not accept additional coded data in the summary itself but
information relating to the gold standard for palliative care[^3] may be
uploaded if the patient gives prior consent.

Wales are deploying an Individual Health record, which has been
implemented in Gwent and is now available to other Health Boards for
rollout. Northern Ireland are also developing an Emergency Care Summary
which should be rolled out to the Southern Trust during 2011.

### 8e.2 Consent {#e.2-consent .ListParagraph}

The consent models for the SCR[^4] and ECS[^5] are similar but differ in
some details. For the SCR, a core extract is sent on the basis of
implied consent. Access is allowed only if the patient gives explicit
consent but that consent requirement may be overridden in the case of
emergency (where, for instance, the patient is comatose). Each patient
may opt not to have a summary care record (and to have existing records
deleted subject to a board review). If they opt to have an SCR, then
they may decide to require to be asked each time it is accessed - or to
give free access to those responsible for their care. The former option
is the default one. For each patient his or her consent status is
recorded on the local system using a flag or Read code. It is clearly
important to record that status accurately so that, on the one hand,
information is included in the SCR that should be, and on the other,
that information is not sent when the patient has opted out.

Adding further codes/text to the record will only occur on the basis of
a decision taken by the clinician/patient and requires explicit consent
by the patient.

For the ECS, a core extract is sent on the basis of implied consent.
Access is also determined by explicit consent except in the case of
emergency. No enrichment of the ECS record is currently possible except
in the case of palliative care settings. In the latter case, explicit
consent needs to be given before the upload of the agreed dataset.

### 8e.3 Data quality {#e.3-data-quality .ListParagraph}

The general requirements for data quality described elsewhere in this
document apply (see also chapter 6). Some specific considerations are
detailed below:

### 8e.3.1 Medication {#e.3.1-medication .ListParagraph}

It should be recognised that the remote user of the SCR/ECS will not
have access to the whole source record or, in most cases, familiarity
with the patients concerned. In these circumstances, it is more than
usually important to ensure the completeness and accuracy of the
medication record by;

-   *Engaging in timely medication reviews*

-   *Entering handwritten prescriptions in the electronic record*

-   *Entering medication prescribed and dispensed in another care
    setting*

-   *Entering regular OTC medication where possible*

### 8e.3.2 General clinical codes {#e.3.2-general-clinical-codes .ListParagraph}

Where it is decided to add codes and text to a summary care record
beyond the core set, it is highly desirable that this should be done as
consistently as possible so that the end clinical user of the record may
have some confidence in the reliability of the information presented
both in terms of what would be expected to be included and what would
normally be excluded.

Clearly, there will be some differences in enriched records both because
different platforms handle the summarisation of record content
differently, and because different users will adopt different
conventions of usage of their systems.

Having said that, the RCGP has produced a set of recommendations[^6] for
the enriched content of the GP Summary in the SCR which include the
following general categories:

-   *Major diagnoses*

-   *Conditions that may have a chronic or relapsing course*

-   *Conditions for which the patient receives repeat medications*

-   *Conditions that are persistent and serious contraindications for
    classes of medication*

-   *Major operations*

-   *Significant therapies & treatment plans*

-   *Significant investigations*

-   *Fractures*

-   *Immunisations*

How this is achieved will, to some extent, be platform dependent.
However, in order to reach this end, some general requirements will need
to be present including:

-   *Practices will need to have a reliable and timely process for
    summarising the records of new patients*

-   *Practices will need to have a comprehensive policy for capturing
    significant diagnoses and events made or occurring in primary care*

-   *Practices will need to have a reliable process for coding
    significant diagnoses and events made or occurring in other care
    settings*

-   *Practices will need to maintain the completeness, relevance and
    contemporaneousness of local problem lists*

Finally, it is important to recognise that the ultimate responsibility
for the completeness and accuracy of the content of the SCR/ECS will
rest with the authors of the source (GP) record.

In addition to the need to include clinical codes consistently, there is
a similar equivalent need to exclude sensitive data. An exclusion
dataset has been defined for use by suppliers so that a range of codes
relating to sexually transmitted diseases/HIV, human
fertilisation/embryology, abortion and gender recognition will be
automatically excluded from any SCR upload. That dataset will be subject
to ongoing review and it may be overridden by patient/clinician
agreement if the patient decides to share items that otherwise would not
be included in the SCR.

There may, of course, be information outside these areas, which might be
deemed to be sensitive either generally or in individual circumstances.
In such cases, responsible clinicians will need to flag such entries as
"not for inclusion" in a summary care record. The mechanism for doing
this will vary from platform to platform (See also Chapters 6, 7, 9 &
12).

### 8e.3.3 Smartcards {#e.3.3-smartcards .ListParagraph}

As with all other spine functions in England, access is determined by
smartcard usage and the role based access permissions associated with
them (see also chapter 4). Record entries made when not logged on using
a smartcard or using the wrong role will not update the summary care
record. The consequence of this is that the summary will not be updated
in line with the local record, resulting in potential clinical error if
decisions are made on the basis of erroneous information. The
consequence of this is that it is important to ensure that all clinical
users including temporary staff have smartcards with appropriate role
based access when entering clinical data.

[^1]: <http://www.connectingforhealth.nhs.uk/systemsandservices/scr>

[^2]: <http://www.ecs.scot.nhs.uk/>

[^3]: <http://www.gsfs.scot.nhs.uk/documents/GSFS%20palliative%20care%20OOH%20summary%20form.doc>

[^4]: [www.connectingforhealth.nhs.uk/systemsandservices/scr/staff/impguidpm/ig](http://www.connectingforhealth.nhs.uk/systemsandservices/scr/staff/impguidpm/ig)

[^5]: <http://www.connectingforhealth.nhs.uk/crdb/boardpapers/agenda_item_11_2_ecs_report_200505.doc>

[^6]: <http://www.scimp.scot.nhs.uk/documents/RCGPSummaryCareRecordGPSummaryFinal.pdf>
