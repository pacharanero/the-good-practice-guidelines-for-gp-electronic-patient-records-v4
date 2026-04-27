---
title: 8b. GP2GP Electronic Record Transfer
---

# 8b. GP2GP Electronic Record Transfer

Now more than 58% of all English GPs have the facility for electronic
transfer of patient records between practices GP2GP record transfer
enabled (as at Oct 2010), the GPGv3.1 appendix -- 'GP to GP record
transfer' has been updated and brought into the main body of these good
practice guidelines. While the GP2GP record transfer project continues
in development specific advice (which will be updated from time to time)
will be made available[^1]

### **8b.1 The rationale for electronic GP2GP record transfer**

The overwhelming majority of U.K. general practices now use their
computer systems for recording patient record information in whole or in
part. The GP electronic record was \"legitimised\" in 2000 following the
construction of a previous version of these Good Practice Guidelines.
Paradoxically, the widespread use of electronic patient records has
resulted in deterioration in the completeness and integrity of patient
record information at the point of transfer of care between practices.
This results from a variety of causes whose main headings are;

-   *Patient records that are an unpredictable mix between paper and
    electronic.*

-   *The inability to transfer the electronic part of the record except
    as a print-out from the 'old' practice and the consequent need to
    re-key information (with its associated error factors) at the 'new'
    practice.*

-   *Variable professional skills and assiduity in recording information
    within both paper and electronic versions of the record*

-   *The abandonment of paper as the medium for the prime record in
    favour of the electronic medium*

The net effect of the above places difficulties on 'new' practices in
identifying salient information in transferred records and in
incorporating that information within the new record. This is to known
to have significant (but un-quantified) resource implications for
practices. There is also widespread anecdotal evidence of resulting
adverse effects on patient care.

The rationale for the electronic transfer of records is therefore;

-   *As a support for electronic records in general practice and their
    general benefits in terms of decision support and audit/governance
    abilities.*

-   *To obviate the need, as far as possible, for re-keying of
    paper-based information for new patients and thus reduce resource
    implications*

-   *To reduce the risks to patients arising from the transfer of
    confusing records*

-   *To support the continuity of electronic patient records as the
    patient moves from practice to practice*

### **8b.2 The nature of electronic GP2GP record transfer**

Electronic patient record systems in general practices in England are
provided by the commercial sector. They are regulated by GP Systems of
Choice (GPSoC). At the time of writing this update to the Good Practice
Guidelines, six different commercial suppliers are known to be involved
in this provision[^2]

Each of the systems so provided is designed differently and older
systems were not constructed with the requirements of clinical data
interchange in mind. In consequence, the data structures and data views
are heterogeneous (see discussion in the Data Transfer chapter 8.2) and
so there is no single simple mechanism that can be constructed that will
allow the passage of structured clinical data of 100% accuracy and
integrity between these different systems.

GP2GP record transfer is carried out using an electronic message, which
specifies a common \"architecture\", expressed using the HL7 standard,
into which the various systems concerned may map their data structures
in a form which is mutually comprehensible. What this means in simple
terms is that there is a common convention for the representation of;

-   *Record Encounters; what constitutes a single transaction with the
    record such as a surgery consultation, a letter received from
    outside the practice, an investigation result etc.*

-   *Names for these encounters; e.g. Home Visit, OOH Consultation,
    Surgery Consultation etc.*

-   *Headings within these encounters*

-   *Complex clinical constructs; e.g. Investigation batteries, Blood
    Pressure Results etc.*

-   *Code mappings; e.g. from various sets of medication codes*

-   *Codes and associated text*

-   *Major modifiers of clinical meaning; e.g. Uncertainty, Allergy,
    Family History*

In addition, there are rules, which require the degradation of
structured clinical information to text where, in any instance of a
record transfer, it is not possible for a system to safely map into or
out of this common structure.

The net effect of the above is to allow records to be transferred in a
form which is 100% human readable and preserves as much of the structure
of the record as possible thus reducing the need to re-key information.
There remain, however, some elements of current electronic records,
which cannot currently be transferred in completely structured form in
every case because of different conventions for describing them on
different systems or different coding schemes used.

### **8b.3 The limitations of electronic GP2GP record transfer**

There are four particular aspects of current GP records where the record
transfer process needs to be supplemented by additional rules or
processes if fully safe and usable records are to be reconstituted on
receiving systems. There are also further limitations to be aware of
that affect the appearance / usability of the record.

### **8b.3.1 Medication information **

There are currently three different coding schemes for the
representation of medication information on GP systems. Transfer of that
information can be achieved by adherence to a combination of rigorous
mapping rules and associated automated machine checks against those
rules. Experience within the GP2GP record transfer project showed that
adherence to those rules allows for a very high degree of reliability of
transfer -- approaching 100% but, crucially, not actually reaching that
point.

The principal reasons for failure to reach 100% reliability are;

-   *The multiple coding schemes used and*

-   *Failure of previous code mapping exercises (see Data Transfer
    chapter)*

-   *The multiple coding scheme problem cannot be overcome until the NHS
    implements a common coding scheme for drug information on all
    electronic record systems. Even then, however, there can probably
    never be a guarantee that legacy medication information held on
    computer systems was always reliably coded, particularly when those
    codes resulted from a historical code mapping exercise. While this
    is a problem that will reduce over time following the introduction
    of a common coding scheme, it has effects on record transfer
    expectations and associated good practice, which are discussed
    below.*

In addition to managing medications that do not transfer automatically,
there is a need to transfer the responsibility for prescribing to an
appropriate user at the 'new' practice. GP2GP applies the following
rules;

-   *Repeat medications which were 'current' at the time when the
    patient left the 'old' practice will be de-activated on import*

-   *Review dates will not be transferred from 'old' to 'new' practice*

-   *Suppliers will offer the means to users with appropriate
    prescribing rights easily to identify and re-activate / authorise
    'current' medications selectively*

-   *Any 'current' medication that has been degraded to text will be
    brought to the user's attention *

Past issues of medication are normally grouped in EMIS systems but this
grouping is lost when the data is imported back into EMIS system.

DM + D is now the preferred standard for handling medicines and devices
and all current GP systems are capable of mapping such information to
and from DM + D. The trend towards DM + D becoming increasingly
integrated into GP systems has been accelerated by projects such as
Electronic Prescribing Service (EPS).

### **8b.3.2 Allergy information **

For a number of reasons it is not currently possible in every case to
exchange information about drug allergies between all systems in a way
that preserves interaction with prescribing decision support.

Within the GP2GP record transfer project a set of rules has therefore
been constructed which allows for every instance of a recorded allergy
to be clearly identified as such[^3] and, when the associated
information cannot be incorporated directly into a different receiving
system, for this information to be presented to the user so that it can
be modied into a form which conforms to that required by the receiving
system -- the aim being to ensure that this allergy information will
trigger appropriate warnings during future prescribing events.

**It is essential that practices understand clearly and unambiguously
that to be interoperable (in the GP2GP sense) adverse drug reactions
MUST be entered in a way that interacts with the native prescribing
decision support system - and that users MUST enter the information
relating to degraded adverse drug reactions in an imported record in
such a way that it interacts with their clinical system prescribing
decision support software.**

(See also Chapter 6.6.1)

Any drug allergy information which has been degraded to text or which
cannot be properly represented on the receiving GP system as an allergy
will be brought to the user's attention.

**For reasons of clinical safety it will not be possible to issue any
medication on the receiving system until appropriate action has been
taken for every drug allergy degrade and the degrade has then been
deleted.**

### This has implications for good practice, which are discussed below.

### **8b.3.3 Business specific information **

There are and will be from time to time, aspects of GP electronic record
keeping that are designed to support specific business processes
relating to terms and conditions of service and/or remuneration such as,
currently, Quality and Outcomes Framework (QOF), immunisation and
cervical cytology call/recall/targets. For most of such processes,
either different systems have different conventions for their
representation or users create idiosyncratic methods for handling them
or both. This has two broad consequences at the point of transfer of the
information.

Firstly, while it is always possible to transfer the raw data that
supports, for instance, cervical cytology call and recall between
systems, it may not be the case that information can be recreated on a
receiving system so that it supports that system\'s own call and recall
functions. During the course of the GP2GP record transfer project, a
general template for handling cervical cytology information was proposed
but this has not yet been implemented and, until such a common view is
held, practices will continue to have to do additional work to make such
information completely useful when received from a different system.

Secondly, individual practices may create internal reports to support
things like target payments based upon an internal practice agreement as
to what codes will be used. These code-lists will not necessarily be the
same as those used by a receiving practice following transfer.

The good practice effects of this are discussed below.

### **8b.3.4 General record view **

**Users should be aware that information imported via GP2GP from a
previous practice may not obey rules on the receiver system, in terms of
appearance, layout or ordering, to which users are accustomed. This will
necessitate some changes in the way that records are viewed so that
important information is not missed.**

As discussed in the Data Transfer chapter, transfer of information
between different systems will result in an alteration in the way that
information is viewed and navigated by the receiving system. This does
not necessarily have any adverse effect upon the process of patient
care, provided that clinical users of the systems understand that this
is the case and interpret the record accordingly.

-   **Duplication, transfer degrades and order changes**

One of the inevitable consequences of heterogeneous record transfer
(transfers between different types of GP system) is that the incoming
record may have a very different appearance on the receiving system from
that on the sending system. This is because the receiving system will
not always be able to replicate structures native to the sending system.
Where structures (e.g. Vision forms) cannot be faithfully represented on
the receiving system their content will be imported and displayed as
text. This text will typically be a concatenation of the field
descriptions and entries from the original form. Sometimes the same (or
similar) information may be displayed twice. Where information is coded
in the incoming record using a coding system that is not recognised by
the receiving system (e.g. Egton code or Emis drug code) the information
will be converted into a transfer degrade. In the receiving system the
original text will be displayed but the original code will be replaced
with the most appropriate transfer degrade code. The sending system may
be able to support consultation entries that string together sequences
that consist of text followed by code followed by text etc. A receiving
system that can only display one code at a time followed by one piece of
text will typically re-order the information displaying each code on a
new line followed by its original text followed by a label 'prefix text'
followed by the prefixed text. Despite these duplications, degrades and
order changes the original meaning is usually clear. There is no need to
edit out these irregularities

-   **Local codes and transfer degrades**

There are broadly two kinds of local codes;

-   *System wide and managed by the Supplier. *

-   *Practice generated. *

The former can be transferred without degrade where sending and
receiving practices use the same system. However, they lead to transfer
degrades in any other (i.e. heterogeneous) transfer. In the interests of
improving the quality of record transfers suppliers are being asked to
reduce the use of these codes. Practice generated codes will always lead
to transfer degrades so that their use should be strongly discouraged.
Where they have to be used the associated text should always have a
clear, unambiguous meaning that will be understandable to any user in
the future, bearing in mind that the patient may change to a different
practice.

-   **Consultation structures**

No two types of GP computer system support the same consultation
categories and at least one system offers no categories at all. Because
these cannot be rendered completely interoperable this results in items
being displayed under unusual categories and also to changes in ordering
when compared with the sending system. However, typically the original
meaning is easily understood.

-   **Values, units, ranges, and abnormality indicators changed to
    text**

Units are not fully interoperable between different systems. Where a
receiving system cannot 'understand' units, the value, units, range and
abnormality indicators may become converted to text. While such strings
may be perfectly understandable to humans it is important to understand
that the machine will not be able to handle values converted to text
(e.g. when running searches or showing a sequence of results
graphically).

-   **Cross mapping limitations**

At present not all systems involved in GP2GP record transfers use the
same coding system for representing medications but all systems are
capable of translating medication information between their native
medication coding scheme and DM + D. However even the best quality cross
map breaks down where a medication cannot be represented either in DM +
D or in a native coding scheme resulting in medication transfer
degrades. Any receiving system following GP2GP processing rules should
be able to recognise medication transfer degrades and display these in
the appropriate part of the record. The original term text should be
preserved so that the original medication entry will at least be human
readable. Thus when medications are initially reviewed appropriate
action may be taken.

In future it is possible that clinical information will be transferred
between systems using different coding schemes (e.g. Read v2, CTV3, or
SNOMED). This will inevitably act as a potential source for further
transfer degrades.

-   **Linkages between different elements of the EPR**

While best attempts have been made to extract information about linkages
between different elements of the record it has proved difficult to
reconstitute these reliably. Some elements that the user might normally
expect to find linked may not be so. As examples, linkages to problem
headings and to referral documents will not be fully reconstituted on
the receiving system. This may necessitate searching the record more
thoroughly (e.g. for relevant documents) than might be necessary for a
'native' record

-   **Degrades to text**

These will occur where an importing system cannot effectively emulate
structured information and this is mainly a problem where sender and
receiver systems are different. The rule is that such information will
be degraded to human readable text which will preserve the meaning.
While human readable meaning may be preserved any automatic function
dependent on structured as opposed to textual entries will be lost.
There are various situations where this may occur and the following are
examples:

-   *Term Codes: Some term codes exported from EMIS systems cannot be
    recognised on import to InPS Vision and so are degraded to text.
    This may occur where term codes have been used in the process of
    migrating EMIS practices from 4 byte Read to Version 2 Read*

-   *Qualifiers: Some InPS Vision forms carry qualifiers which are
    extracted as text. On import to an EMIS system the forms cannot be
    reproduced so that the qualifier information appears as text*

-   *Dates: Some InPS Vision forms carry contextualised dates (e.g.
    disease register forms) which will be degraded to text on import to
    an EMIS system Medications: Some medications (e.g. mixtures) cannot
    be represented in the NHS standard Drugs, Medications and Devices
    dictionary (DM + D). Where sender and receiver systems are different
    the details will be degraded to text*

-   *Allergies: Where drug details cannot be represented in DM + D and
    the sender and receiver systems are different, the details will be
    degraded to text*

<!-- -->

-   **Dates**

Typically, observations in GP records are displayed with a single
uncontextualised date usually on the left hand side of the screen. This
date may have been changed by the user at the time of data entry for a
variety of different reasons (e.g. the observation was made on a date
that differs from the system date). In most cases this will not have
important clinical consequences. However, it should not be assumed that
other practices will change these dates according to any particular set
of rules. Therefore dates that are not associated with an explicit
context should be interpreted with care. Some dates do have a clear
context (e.g. plans, recalls) both in sender and receiver systems.

InPS Vision holds contextualised dates in a small subset of its forms
(e.g. 'date of last fit'). Where the record is transferred between InPS
Vision systems the display of these dates will be preserved in context.
Where the record is transferred to any system that can only handle one
date (e.g. EMIS LV system) such dates will be degraded to text which
will be displayed with the rubric and any other text. Thus in text the
context of the date will be preserved. The left hand date may be changed
to this same "effective date".

It is hoped that in future GP systems will be better able to
contextualise dates and that future versions of the message will be
better able to handle that context.

-   **Complex consultation text -- EMIS system **

EMIS users in Consultation view can construct complex strings of text
and coded information. This construct can be passably recreated on
re-import to an EMIS system but users may see line returns in unusual
places.

It has proved very difficult to represent this construct meaningfully
when the information is imported to an InPS Vision system. Currently
InPS Vision users will see a series of coded entries interspersed with
text. Code and text may not appear in the same order as in the
originating EMIS system, which can sometimes make such entries difficult
to interpret. Selection of a different record view may help. Further
work is in progress to ameliorate this.

### **8.3.3.5 Attachments including Documents**

The GP2GP definition of an attachment includes any file that is separate
from the main body of the electronic record but with an explicit link
embedded in the record. This link must enable the location of the source
file to be identifiable from within the record. All such attachments
should be extracted in parallel with the main body of the record and
transferred by the GP2GP transfer process to the next practice. At the
receiving practice all such attachments should be accessible from within
the record once it has been filed. However, there are currently
limitations;

-   *The Spine Transaction and Messaging Service (TMS) currently only
    operates with a restricted list of file types. Where an attachment
    is of an unsupported file type it cannot be sent across the TMS to
    the next practice. In such a case a 'placeholder' will be sent
    instead of the file*[^4]

-   *The TMS currently has a message size limit of 5 Mb. If the total
    size of the record plus all attachments exceeds this limit then the
    GP2GP record transfer will fail totally*[^5]

-   *The TMS currently limits attachments to a maximum of 99. If this
    limit is exceeded then the GP2GP record transfer will fail
    totally*[^6]

-   *Some Third Party document management systems employ their own
    application programming interface (API) to interpret the address in
    the embedded link in order to determine the true location of the
    file. Unless the GP system supplier can access this API at the time
    of extraction the file will not be found. In this case only a
    placeholder will be sent on to the next practice*[^7]

-   *Contextual information (e.g. meaningful name or descriptive
    notation) is not currently interoperable between different GP
    systems so that at the receiving system it may be impossible to tell
    the nature / content of any document without first opening it. At
    present this limitation is unavoidable because no standard for
    naming and categorising documents operates in the GP domain*

**8b.3.6 Handling of pathology (PMIP) results **

-   **Dates **

PMIP results may have as many as four associated dates when received
from the pathology laboratory. However, because the present GP2GP HL7
message cannot contextualise dates, this limits the number of dates that
can be forwarded to the next practice to just one. The rule adopted sets
this as the date that the specimen was received by the laboratory.

-   **Units, ranges and abnormality indicators **

PMIP results when transmitted from the pathology lab will typically be
accompanied by their own units, normal ranges and where appropriate,
abnormality indicators. These will vary from laboratory to laboratory.
For individual results to be correctly interpreted it is therefore vital
that this information be preserved as originally sent. The rules adopted
for GP2GP transfers of PMIP data are as follows:

-   *The PMIP units, ranges and abnormality indicator (if present) as
    originally received from the laboratory must be extracted from the
    'old' practice and sent along with the value of the result to the
    'new' practice*

-   *On import, the 'new' practice system must preserve PMIP units,
    ranges and abnormality indicator (if present). It must not
    substitute 'native' units or ranges nor change the abnormality
    indicator or insert an abnormality indicator where none was
    originally sent by the laboratory*

While these rules will facilitate human interpretation of individual
results they may not assist machine interpretation for example where
automatic searches are performed on values without taking into account
differing units and ranges.

### **8b.4 General clinical safety **

Systems engaging in GP2GP record transfer are required to adhere to some
processing rules on receipt to reduce the potentially adverse effects of
the above limitations (see also Chapter 3)

### **8b.5 Electronic and paper GP2GP record transfer **

The transfer of paper GP records alongside electronic ones will continue
for the foreseeable future for a variety of reasons, which include;

-   *The variable penetration of use in general practice of electronic
    records for direct patient care*

-   *The majority of patient information from outside practices remains
    paper-based*

-   *The variable degree to which such external information is
    incorporated into the electronic record*

-   *The variable degree to which historical patient information native
    to practices has been incorporated into electronic records*

***The net effect of this is that, while electronic record transfer will
reduce the need to re-key information, it will not remove the onus on
receiving practices to enter historical information present in old paper
records if deemed appropriate and clinically significant.***

However, when a patient deregisters and re-registers elsewhere and GP2GP
record transfer is active, the EPR will typically be sent to the 'new'
practice within minutes of re-registration while the request from the
Primary Care Organisation (PCO) for return of the paper notes will not
arrive for days / weeks. If in the interim the 'old' practice has clear
evidence that the 'new' practice has successfully imported the EPR
received via GP2GP transfer (e.g. receipt of a transactional message
from the receiving practice acknowledging that the GP2GP process led to
the EPR being successfully imported)[^8] then in this case there would
be no 'good practice' requirement to print out the EPR and place it in
the Lloyd George envelope. In all other cases the EPR should continue to
be printed out. Practices should be aware that they will need to seek
permission from the PCO to transfer patient records to the next practice
by a medium other than paper.

### **8b.6 GP electronic record quality **

However carefully electronic records are kept, errors in their content
will sometimes be present. The following examples are already known to
have occurred;

-   *Erroneous codes added by a secretary from an inbound letter*

-   *Erroneous diagnostic code added by a doctor on "hearsay" from a
    third party*

-   *Erroneous codes added as a result of a flawed data transfer mapping
    exercise*

-   *Automatic code entry as a result of software misinterpretation of
    inbound electronic messages*

-   *Missing or incomplete significant data*

-   *Data summarised from Lloyd George notes that relates to a different
    patient\'s clinical information *

(see also Chapter 6)

### **8b.7 GP2GP record transfer - good practice guidelines**

The following guidelines apply to the electronic transfer of GP records
in current technical and organisational circumstances. As practices
increasingly move to full electronic records, the NHS moves to an
e-commerce basis, and NHS computer systems are supported by common
terminologies and architectural principles, these guidelines will
change.

### **8b.7.1 Workflow **

### **8b.7.1.1 Links with registration business process**

The GP2GP record transfer process, although triggered by the patient
registering at a new practice, is quite separate from the registration
process. The message transfer process employs the Personal Demographic
Service (PDS)[^9] and the Spine Directory Service (SDS). A number of
checks are carried out to ensure that the correct record will be
requested for the correct patient from the correct previous practice and
that the patient has registered at a genuine practice. The electronic
message carrying the patient's record is conveyed securely across the N3
network into the Transaction and Messaging Spine (TMS) and then out
again across the N3 network to the new practice. Only users with the
appropriate role / access level will be able to trigger the GP2GP
process and even then, only if they have logged on to the system using
their smart card.

A chain of events is triggered when the patient registers. Firstly the
Personal Demographic Service (PDS) is used to run a patient trace. By
using key information such as surname, date of birth, sex, and NHS
number, the correct patient is identified on the PDS. Following this,
the patient's previous practice is automatically identified. An
automatic check is performed using the Spine Directory Service (SDS),
which holds essential information about NHS organisations, to find out
the exact electronic location of the previous practice and to check
whether or not it is GP2GP enabled. If the previous practice is not
GP2GP enabled then the GP2GP process stops and the registration process
simply reverts to a paper based record transfer. If the previous
practice is GP2GP enabled then an electronic request is sent to the
previous practice using the EHR request message.

At the previous practice a series of events takes place automatically;

-   *A check is performed to confirm that the patient's record can be
    found*

-   *If the record is found then a check is run against the SDS to
    obtain the routing details of the patient's new practice*

-   *An electronic acknowledgement is sent to the new practice*

-   *A check is run against the PDS to check that the patient has in
    fact registered at this new practice*

-   *Finally, assuming that the previous checks have returned
    satisfactory responses, the patient's electronic record is
    automatically extracted and conveyed by the EHR extract message
    across the N3 network and the TMS to the new practice*

The GP2GP record transfer process is designed automatically to fetch the
patient's record safely, securely and quickly from the previous
practice. Typically the record will arrive within minutes of the patient
completing registration (See also Chapter 8a)

**8b.7.1.2 Automatic sending of the record by the previous practice**

At registration when patients sign the GMS1, or similar locally devised
form they are effectively instructing the new GP to retrieve their
records. It can be argued that neither the previous nor the new GP have
any \'say\' in the process: the new GP is in effect being instructed to
get the patient\'s records. This explicit statement gives the new GP the
right to extract the newly registered patient\'s records whether the
records be paper, electronic or otherwise. For these reasons the strict
legal and regulatory arrangement is that as soon as the patient is
accepted by the requesting practice, they have assumed responsibility
for the patient. From that point onwards the patient is no longer a
patient of the sending practice and that practice has no right to deny
the registered GP access to what is now his patient\'s record.

During the development of the GP2GP record transfer process two issues
were considered;

-   *Whether to have an automatic process that extracted the record from
    the sending practice without intervention from the sending practice,
    or whether to have the sending practice \'allow\' the request and
    determine whether the record would be extracted, i.e. in some way be
    able to stop or deny the request*

-   *Whether the extraction should occur immediately or at some other
    (delayed) time, e.g. 24 or 72 hours later. *

These issues were considered and debated by the full General
Practitioner Committee, the Royal College of GPs, the GP2GP Project
Board and the GP2GP Clinical Safety Team. The unanimous view of all of
these bodies was that the electronic record should be extracted and
sent, automatically and immediately, in response to the EHR request
message.

**8b.7.1.3 Handling of electronic patients received in error**

This guidance has been developed by the GP2GP project and the Joint GP
IT Committee to advise practices how to reduce the risk of making an
erroneous record transfer request and advising practices and PCTs how to
manage such erroneous requests when they do occur. Erroneous record
transfers usually occur when patients are incorrectly identified when
registering with a new GP practice. This may result in a request being
made for the wrong record via a GP2GP transfer and a patient being
inappropriately deducted from their true registered general practice.

-   **Registering new patients **

Correctly identifying and registering new patients on the demographics
database (PDS) is the absolutely key step in reducing the risk of
erroneous GP2GP record requests being made. When completing the GMS1
registration form, practices should carefully check the accuracy of
patient data and try to provide as much information as possible,
preferably including the NHS number when it is available. The GMS1
should be checked in the presence of the patient to check its
legibility, completeness and accuracy. If a patient cannot be positively
identified, practices might consider asking registering patients to
provide formal identification and proof of recent address to ensure that
correct GP2GP record transfer occurs. If in doubt, registration should
be deferred and advice sought from the PCT/Patient Services Agency.

-   **Erroneous transfers & the sending practice **

Most erroneous transfers come to light when the patient contacts their
practice (the sending practice) for an appointment or prescription, to
be told they are no longer registered. Sending practices should contact
their system supplier helpdesk to report the erroneous transfer. The
practice should also contact their PCT (Patient Services Agency) to
request that the patient's registration be reinstated and consider
informing the patient what has happened.

-   **Erroneous transfers & the receiving practice **

The practice requesting the record (the receiving practice) may also
identify that they have the wrong record, or are informed by their
supplier helpdesk that they have registered the wrong patient. Practices
should contact their PCT (PSA) to advise them of the erroneous transfer
and with the support of the PSA and supplier helpdesk, arrange to delete
the erroneous NHS number and "roll back" the clinical system so that the
erroneous incoming GP2GP record is deleted and no patient details remain
in the receiving practice. The receiving practice should consider
whether an erroneous transfer should be considered as a practice
critical incident, to reduce the risk of further such errors.

**8b.7.1.4 Arrangements for returning patients -- the 'A -- B -- A'
scenario**

Where a patient returns to re-register at Practice 'A' the previous
electronic record including demographic entries should still exist. This
forms a special case known as the 'A -- B -- A' scenario and leads to
the following challenges:

-   *Practice 'A' must not end up with duplicate records for the patient
    (i.e. both the original and the newly received records). *

-   *The need to keep duplication, disorganisation and degradation of
    the content of the original existing record at Practice 'A' to a
    minimum when attempts are made to merge this with the incoming
    record from 'B' *

-   *The need to apply all changes to the record deliberately made by
    any user since the patient left Practice 'A'*

-   *The need for any merging process to have an automatic default that
    is deemed to be clinically safe*

At the present time these challenges cannot be satisfactorily met.
Therefore a constraint is applied. Until further notice users should
expect that GP2GP record transfers will not take place for returning
patients. Instead, the original record at 'A' should be reactivated.
Work is currently in progress to develop an intelligent, safe 'merge' of
records for returning patients. The main aim will be to preserve all of
the changes that have resulted from deliberate actions by a clinician
since the patient left Practice 'A' but to minimise the duplications,
degrades and disorganisation to the pre-existing record (at Practice
'A') that result from the automatic processes of heterogeneous GP2GP
record transfer (transfers between different GP systems). A secondary
but important aim will be to maximise the chances of achieving long,
unbroken chains of electronic record transfers and generally to improve
the quality of these transfers.

**8b.7.1.5 Parallel running with paper records**

At this point in time although the number of non-computerised practices
is very small a significant part of the GP estate in England is not
GP2GP enabled. Nor are there arrangements in place for cross border
electronic record transfers. For this reason paper records must continue
to follow the patient. GP2GP enabled practices remain contractually
bound to follow standard practice for the handling of paper records. For
guidance about the need to print out the EPR see section 8b.5
'Electronic and paper GP2GP record transfer'.

**8b.7.2 Organisational implications of the GP2GP record transfer
process**

The GP2GP record transfer process can be considered in a series of
stages each of which needs to be supported organisationally by the
practice. The precise details as to how these stages should be managed
and by whom will depend on the practice. However, particular attention
should be paid to the checks outlined in section 8b.7.5 and the general
principles enumerated in section 8b.7.6 should be followed. The stages
might typically follow in this sequence:

1.  **Registration process / PDS trace and triggering of the automatic
    EHR request process: **

> It is vital that staff involved with the registration of patients
> should understand the process, and the need to be logged on with Smart
> card. To minimise the risk of mismatching patients they should be
> thoroughly trained in the use of the PDS trace. (See section
> **8b.7.1**). In this context, they should be aware of the importance
> of using the patient's NHS number wherever possible.

2.  **Initial check of incoming records leading to filing in a timely
    fashion: **

> All systems provide a facility to preview the incoming record before
> it is filed into the database. Some systems provide facilities to
> filter this preview in various ways (e.g. to identify drug allergy /
> medication degrades) and to give an impression of the overall quality
> of the record. The record should be checked to ensure that it is not
> obviously the wrong record for a patient of the stated age and gender.
> It is not possible in any way to alter the incoming record at this
> stage. However, in exceptional circumstances (e.g. if this turns out
> to be the wrong record or if the record is deemed to be of such poor
> quality as to be useless), the user has the option to reject the
> record and to opt for the Practice to start building a new record from
> scratch. In the majority of cases the aim should be to file the record
> without delay so that the patient and attending clinicians can benefit
> from having access to the record as early as possible (e.g. have
> access to information about current medications and drug allergies).
> Any entries that have been made to the patient's record prior to
> filing should be checked against the previous record after filing and
> any inaccuracies or duplications should be appropriately handled. It
> follows that the earlier the record is filed the less the amount of
> checking that will need to be done.

3.  **Fixing of any degraded drug allergies in the incoming record so
    that prescribing is unlocked**

> The GP2GP record transfer process has been designed to minimise the
> risk of drug allergy information being lost or over-looked leading to
> inappropriate prescribing. Because drug allergies are represented in
> different ways in different systems it is inevitable that degraded
> drug allergies will occur. These will not interact with prescribing
> decision support. ***After filing, the presence of even a single drug
> allergy degrade will therefore lock down prescribing making it
> impossible for any medication to be authorised / prescribed until the
> degrades have been appropriately processed.*** Different systems
> provide users with different tools to identify these degrades, to
> enter the allergy in the appropriate way, and then to delete the
> degrade. These actions are recorded in the system audit trail. It is
> vital that everyone who has access to the record before these degrades
> have been processed fully understands the importance of handling them
> in the proper way. Following preview and filing some practices may
> choose to give the processing of these degrades a high priority so
> that time can be saved in the first consultation.

4.  **Reviewing and re-authorising medication (typically with the
    patient):\
    **At the first consultation immediately after registration time is
    likely to be at a premium. As a minimum:

    a.  A conscious check should be made to ensure that the demographic
        details belong to the consulting patient and that the correct
        electronic record has been filed into the practice system for
        this patient.

    b.  The accuracy and appropriateness of current medications and
        allergies should be checked with the patient. ***N.B.
        Medications may not be prescribed from an incoming record
        until;***

        i.  ***All drug allergy degrades have been processed (see
            above)***

        ii. ***Medications have been reviewed and (re) authorised by a
            prescriber in the new practice***

5.  **General review of the record with the patient to check and correct
    any missing information or inaccuracies: **

> **\
> **The prime objective here is to ensure that from the patient's point
> of view the record is complete and accurate (See section 8b.7.6
> General principles for guidance about making alterations). In
> particular, if not already done;

c.  A conscious check should be made to ensure that the demographic
    details belong to the consulting patient and that the correct
    electronic record has been filed into the practice system for this
    patient

d.  Any interim record information that may already have been entered on
    the receiving system should be checked against the incoming record

e.  Any current medication or allergy information should be checked for
    accuracy

<!-- -->

6.  **Review of paper record to look for and back load missing
    information: **

> **\
> **Typically this will be a 'back office' activity similar to the
> 'summarising' activity performed for paper-based transfers. The main
> objective should be to find important information in the paper record
> that was not entered into the electronic record at the previous
> practice. ***There should be no need to check the computerised
> printout from the previous practice, as the GP2GP process will have
> transferred all of this information.*** It is likely to be more
> rewarding to check for any summary card and to check hospital letters.
> Practice staff should resist the temptation to make cosmetic changes
> to the incoming record (See section **8b.7.6** General principles)

7.  **Business specific information review: **

> **\
> **The aim of this 'back office' activity is to review the record to
> ensure that it contains necessary entries to support practice business
> processes (e.g. cervical cytology call / recall). In this case,
> because individual practices have different ways of managing their
> various business processes it is very likely that changes will need to
> be made to the record. However, these should be kept to a minimum (See
> under general principles for guidance about making alterations to
> incoming records). This activity can be carried out in parallel with
> the other activities outlined above.

8.  **Keeping filing of incoming results / correspondence up to date:**

> In contrast to all of the above points, which relate to the receiving
> of records this relates to the Practice's role as a sender of records.
> Practices often have no advance warning that a patient has moved and
> registered elsewhere. Because GP2GP record transfer is an automatic
> process notification that the record has already have been transferred
> to the next practice may be the first indication that the patient has
> moved (See section 8b.7.1.2 for discussion of automatic sending of
> records). It is therefore good practice to keep filing of all incoming
> results and correspondence up to date. In the event that pathology
> results have been received into the practice and matched but not yet
> actioned, the GP2GP transfer process will forward all such results to
> the next practice. However, the requesting clinician remains
> responsible for ensuring that any action appropriate to a result is
> taken even though the patient has moved on to the next practice. To
> the receiving practice the results will appear to have been actioned.
> To the sending practice the results will still be displayed as
> awaiting action. ***If urgent action is needed it may be necessary to
> contact the new practice. PCTs or PCAs should be able to assist in
> this and practices should be clear about the procedure to be followed
> in such cases.***

**8b.7.3 Training **

Practices should ensure that all of the processes outlined in section
8.3.7.2 are integrated into their general operations and managed
effectively. There should be clear policy about what each of these
functions should entail and who will perform each of them. Roles should
be clearly defined and appropriate system access levels set up,
commensurate with experience, training and responsibility, to enable
users to carry out these roles. The team members concerned should have
undergone appropriate training. In particular:

-   *A responsible member of staff and a deputy should be identified to
    take the lead within the practice and be trained in the processes
    involved in GP2GP record transfer*

-   *The Practice lead should identify how the processes outlined in
    8.3.7.2 will be integrated into general practice operations and
    carry out a training needs assessment of the people involved. In
    particular this should address:*

    -   *Registration process and PDS trace*

    -   *Initial check of records on receipt and filing*

    -   *Handling of drug allergy degrades*

    -   *Reauthorisation of medications / identification of what was
        current medication in previous practice*

    -   *Review of paper records, what to backload, how to achieve this
        keeping changes to incoming record to a minimum*

    -   *Dealing with business specific information*

-   *All users of the practice system should be trained in what to
    expect from electronic record transfer and, in particular, from the
    limitations outlined in section 8.3.3 of this chapter. *

-   *More generally, all members of the clinical team and relevant
    members of the administrative team should be familiar with these
    good practice guidelines prior to commencement of GP2GP record
    transfer*

-   *Practices should identify a date from which they will implement
    GP2GP record transfer and all members of the practice should be
    informed of the date of commencement of GP2GP record transfer*

**8b.7.4 Non-computerised practices **

Although the number of non-computerised practices has become very small
not all record transfers between practices are capable of being covered
by GP2GP electronic record transfer. Therefore it will be necessary to
continue to exchange paper records for the foreseeable future. (See
**8.3.7.1.5** -- Parallel running with paper records)

**8b.7.5 Validation **

> This is about 'fitness for purpose' of the incoming record and relates
> to things that should be done as soon as possible after the incoming
> record is received;

-   *Check that both demographic information and associated electronic
    record relate to the patient*

-   *On preview confirm that the record is of adequate quality to file*

-   *Check compatibility and consistency between any interim record
    already made and the filed incoming record*

-   *Deal with any drug allergy degrades*

-   *Reauthorise medications and deal with any medication degrades*

-   *Check business specific information and amend entries to align with
    practice processes but resisting the temptation to make any changes
    unless they are absolutely necessary from a safety / usability /
    business process point of view*

**8b.7.6 General principles**

-   *The quality issues identified in section 8.3.6 above require
    practices to have in place mechanisms aimed at reducing or
    eliminating the impact of externally received erroneous data.*

-   *The practice\'s natively created record should be maintained in
    line with these \"Good Practice Guidelines for General Practice
    Electronic Patient Records v4\"*

-   *Practices should review their organisational arrangements so that
    they are able to support the processing of incoming records as
    outlined in section 8.3.7.2*

-   *In particular, the incoming record should be subject to validation
    checks as identified in section 8b.7.5 *

-   *Practices should recognise that patients themselves are generally
    the most competent to judge the accuracy of their own historical
    information, and should consider ways of enabling patients to
    comment on the content of their records at specific points in their
    experience such as their first visit after registering, on the point
    of referral to hospital etc.*

-   *Practices are provided with functionality on their systems that
    will allow them to review but currently not to alter incoming
    records before they are filed. They are currently presented with a
    choice of either filing the record into the Practice database or
    rejecting it in which case it will persist as an attachment to the
    patient's new record. The choice to reject should only be exercised
    rarely*

-   *Practices are provided with further functionality to assist them in
    making some essential changes to the record after filing (e.g.
    degraded drug allergies -- see below)*

-   *There is a need to review and, in some cases to make further
    alterations to the information in those records after filing (See
    sections 8b.7.5 and 8b.7.2). When doing this the responsible user
    should ensure that;*

    -   ***Incoming record information is not modified beyond what is
        necessary to make it safe and usable on the receiving system***

    -   ***Incoming record information is never deleted unless deemed to
        be unsafe in terms of its accuracy or comprehensibility***

-   *When paper records are subsequently received they should be
    reviewed by a GP or other appropriately trained member of staff and
    amendments made to the electronic record where appropriate*

[^1]: <http://www.connectingforhealth.nhs.uk/systemsandservices/gpsupport/gp2gp/goodpractice>

[^2]: <http://www.connectingforhealth.nhs.uk/systemsandservices/gpsupport/gpsoc/systems>

[^3]: The GP2GP definition of a 'drug allergy' covers every instance of
    a record entry of an adverse drug reaction that triggers the 'native
    system' prescribing decision support system. The aim is to ensure
    that appropriate entries are made on the receiving system that will
    trigger its 'native system' prescribing decision support system

[^4]:

[^5]: In all of these cases a 'Large Message Solution' is expected to
    overcome these limitations but even so it may still be impossible to
    open some file types in the receiving system if the necessary
    application is not installed

[^6]: In all of these cases a 'Large Message Solution' is expected to
    overcome these limitations but even so it may still be impossible to
    open some file types in the receiving system if the necessary
    application is not installed

[^7]: In at least one case this problem can be solved if the sending
    practice upgrades its document management system to the appropriate
    version. In other cases there may still be work to be done between
    individual document management system suppliers and GP system
    suppliers

[^8]: Unfortunately at the time when these guidelines were being written
    GP2GP version 1.1a did not support the necessary transaction
    messages to support this. However, this may change in which case
    instructions as to how and where the relevant transaction message
    can be found will be system specific and therefore should be sought
    from the system supplier. Note that it will be necessary also to
    resolve the issues relating to file attachments outlined in section
    8.3.3.5

[^9]: http://nww.connectingforhealth.nhs.uk/demographics
