---
title: 3. Clinical Safety Assurance
---

# 3. Clinical Safety Assurance

### 3.1 Introduction

Clinical safety assurance is a broad subject. This section focuses on
the clinical safety approach that applies across the NHS in England,
issues that are relevant to the safe exchange of clinical information
between systems across organisational boundaries, and relevant
standards. This is particularly important in terms of health records
inter-operability and underpins the data transfer and inter-operability
sections of these guidelines (see Chapters 8a-f)

### 3.2 Clinical safety approach

The factors contributing to increased risk have been described[^1] as
including:

Organisational factors;

- *Management decisions*

- *Organisational processes*

- *Corporate culture*

Workplace factors;

- *Error producing conditions*

- *Violation producing conditions*

Personal factors;

- *Errors*

- *Violations*

###

'High reliability' organisations have been identified that are observed
to have less than their fair share of accidents. These organisations
tend to use a 'system approach' that deliberately roots out error traps
and concentrates on the conditions under which individuals work,
designing systems that defend against errors or mitigate their effects.
This contrasts with an alternative approach of waiting for errors to
occur and then laying blame on the individual(s) involved with the
error.

In the English NHS the Connecting for Health Clinical Safety Group (CSG)
has developed the Clinical Safety Approach (CSA). The CSG aims to
nurture an open safety culture that is broadly in tune with the 'system
approach' outlined above, to cover all English NHS information systems.
Thus recently standards have been developed that apply to all English
NHS organisations and to system suppliers. More will follow (see
sections 3.4 and 3.5 below).

It should be emphasised that no system can ever be made completely safe.
In reality it is only possible to reduce risks to levels that are *As
Low As Reasonably Practicable* (ALARP principle).

The CSA is a clinically led process that has three stages:

- ***End to end hazards workshop** to 'walk through' the processes
    with which a software module is associated in order to identify
    those things that may cause harm to a patient*

- ***Development of a clinical safety case** where hazards identified
    are scored for likelihood and impact and prioritised according to
    the resulting risk score. Appropriate 'mitigations' are identified
    and agreed for all of these hazards.*

- ***Safety closure Report**. At this stage evidence is assembled to
    demonstrate that all of the mitigations agreed in the clinical
    safety case have been carried out. The resulting safety closure
    document is presented to the CSG. Various regulations are in place
    to prevent systems from being deployed / released until safety
    closure has been satisfactorily completed*

Despite rigorous application of the Clinical Safety Approach safety
issues may still be identified after a system has been deployed. There
are mechanisms in place to enable users to report any suspected clinical
safety problem so that they can be brought to the attention of the
system supplier and, if necessary, the CSG. There should be a
well-understood process and culture for logging and reporting clinical
safety issues within NHS organisations.

### 3.3 Clinical safety assurance and inter-operability

This is primarily about the exchange of clinical information between end
systems in different organisations through the medium of messaging (e.g.
record transfer by GP2GP or PMIP delivery of pathology results from
laboratories to General Practice). In this situation there is a
particular need to ensure that the original meaning of clinical
information is preserved through successive transfers. Clinicians at
each end of a messaging link are likely to be entering information in
different ways on systems that are heterogeneous (i.e. have different
information models supporting different structures and possibly
different coding systems). In such circumstances clinical information
will inevitably be subject to structural transformations and
translations so that it will have a different appearance with different
ordering / organisation on the receiving system. The arrival of more and
more heterogeneous systems (e.g. PMIP, SCR, GP2GP, EPS) that are
required to interoperate with each other, if not carefully managed and
tested, will increase the risk of change or loss of clinical meaning.
The challenge is to ensure that despite all of these factors clinical
meaning is preserved so that a clinician working on any receiving system
will in a timely fashion be able to find all of the information relevant
to the patient's circumstances, interpret it correctly and make
clinically safe and appropriate decisions.

- *Practice teams will require education and training to understand
    the implications of working in an increasingly interoperable
    environment (see Chapter 12)*

- *The quality of the information held on the originating system is of
    paramount importance as this may impact on the decision making of
    everyone downstream (see Chapter 6)*

- *Rigorous, centrally managed, clinically led safety testing is
    required*

An approach has been developed which depends on trained clinicians, with
delegated professional authority. Specially prepared dummy clinical
records can be compared line by line on side-by-side screens displaying
the same record on sending (i.e. before transmission) and receiving
systems (i.e. after transmission). The records are set up to include
multiple examples of all of the clinical information structures that can
be found on the sending system. This testing is underpinned by a
documented set of clinical informatics principles, which has evolved
over time. It depends on iterations of close collaborative work between
clinicians, technicians, project managers and system suppliers. Wherever
problems are found, attempts are made to run an end to end diagnostic
process to identify the cause, to assess likelihood and impact, and then
full details are captured in an Issues log.

This approach can, and should, be embedded in the CSA. The Issues log is
effectively an extension of the CSA Safety Case. Issues are prioritised
and mitigations agreed. There must be documented proof that these have
been carried out before the CSA safety closure document is issued.

### 3.4 Current NHS safety standards for IT systems (DSCN 14/3009 & 18/2009)

In August 2009 the NHS ISB issued two documents designed to establish a
software safety management regime in the health sector, which is on a
par with safety regimes in similar safety related industries such as
aviation or the nuclear industry. This is directly in line with
statements the CMO (Liam Donaldson) made in his 2006 report in relation
to the NHS "learning from other safety industries".

These safety standards (known as DSCN 14/2009 -- for suppliers and DSCN
18/2009 -- for health organisations) require the proactive risk
assessment and mitigation for IT systems used to support health care,
but which are not themselves classified as a medical device. GP systems
clearly fall into this scope.

The standards are available free and downloadable from the Clinical
Safety Group website[^2]

In summary Health Organisations (and hence GPs) should:

- *Seek to procure systems which comply with DSCN 14/2009 (the
    supplier safety standard)*

- *Carefully risk assess the implications to rolling out a new system*

- *Ensure any risks are properly understood, investigated and
    mitigated by sensible controls (such as checks on migrated data or
    local testing to ensure the new system is correctly configured) and
    *

- *A clear process for reporting safety issues to the system supplier*

The NHS CfH Clinical Safety Group (CSG) provide a more detailed document
which GPs can use as an aide-memoire when changing system -- the Safer
Implementation Guide. This can be accessed here[^3]. This document has
practical information and easily understood checklists to steer a
practice through the key tasks which if conducted result in a
safe-implementation of a new system.

### 3.5 Future Safety Standards including changes to the Medical Device Directive 3.5.1 Changes to the Medical Devices Directive

The Medical Devices (Amendment) Regulations 2008 No 2936 which transpose
Directive 2007/47/EC (relating to amendments to the Medical Devices
Directive) into UK law, were passed by Parliament in December 2008 and
fully come into force in March 2010. This amendment is an update to the
Medical Devices Directive, which may have ramifications for electronic
patient records systems. Any changes to the interpretation of the
Medical Devices Directive will be well publicised via the MHRA web
site[^4]

### 3.5.2 IEC80001

IEC80001 is a new systems safety standard, still under development,
which will emerge over 2010/2011. This standard will place requirements
on a health organisation to properly document and risk assess their
medical IT network. The term medical IT network is only applied to those
systems and network components, which interface with medical devices.
Only those GP surgeries which have interfaces with medical devices
(glucose meters and so forth), where the information from the device is
electronically transferred into the Electronic Patient Record via the
network (wireless or wired) will be impacted.

The requirements of IEC80001 will not be significantly different from
the requirements of DSCN 18/2009, and hence GP surgeries who comply with
DSCN 18/2009 can expect not to be adversely impacted in practise by the
new IEC80001.

The NHS is taking the lead on defining a guidance document for health
care organisations in implementing IEC80001. This will be well
publicised and should be in the public domain alongside the new
standard.

### 3.6 Key clinical safety summary points

a)  Clinicians and other users of NHS systems may at times have
    opportunities constructively to influence decisions that impact on
    organisational and workplace factors that in turn have a systemic
    effect on clinical safety

b)  Mitigations tend to consist of a combination of technical solutions
    and User Guidance. For some hazards, particularly those that are
    dependent on human behaviour or professional 'best practice', the
    only practicable mitigation may be user guidance alone. Users should
    be made aware of this guidance, understand why it has been put in
    place and why it is advisable to follow it

c)  Clinical safety assurance is a distinct and quite separate process
    from usability assurance. Some clinical safety hazards may
    appropriately be identified as low priority and not amenable to any
    practicable mitigation. Users should be aware that a system which
    meets clinical safety assurance requirements may never the less
    still have usability issues

d)  Users should report any suspected clinical safety issues that may
    come to light after a system has been deployed. Primary Care
    Organisations should all have mechanisms in place to enable
    reporting of health IT safety incidents to the National Service
    Desk[^5]. When an issue is reported a National Incident Number (NIN)
    number will be provided

e)  Clinical safety is dependent on clinicians and other users receiving
    appropriate education and training

f)  Good 'data quality' is a very important pre-requisite for safe and
    effective communications

[^1]: Reason JT. Understanding adverse events: human factors. In:
    Vincent CA ed. Clinical risk management. London. BMJ Publications
    1995.

[^2]: <http://www.connectingforhealth.nhs.uk/engagement/clinical/occo/safety/dscn>

[^3]: <http://www.connectingforhealth.nhs.uk/engagement/clinical/occo/safety/guide>

[^4]: <http://www.mhra.gov.uk/index.htm>

[^5]: [**cfh.npfitservicedesk\@nhs.net**](mailto:cfh.npfitservicedesk@nhs.net)
