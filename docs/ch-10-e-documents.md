---
title: 10. Electronic Document Attachments
---

# 10. Electronic Document Attachments

### 10.1 Introduction

This chapter offers guidance on the principles of safe, consistent
handling of attached electronic documents, common document formats,
consistent document identification and the secure transfer of
attachments between practices.

### 10.2 Attached electronic documents

A normal requirement in GP clinical record systems is to be able to
attach an external electronic clinical document to an individual patient
record. A wide range of attached document types and technical formats
may be encountered and the handling of attachments varies somewhat
between GP clinical systems.

'Document attachments' should be distinguished from GP2GP messages, lab
results, and other structured 'clinical messages', which contain coded
and other computer processable information, and whose contents can be
directly imported into the patient record. 'Clinical messages' are
discussed in Chapter 8 (Data transfer & inter-operability).

Some clinical communications e.g. Discharge letters, which are currently
delivered to practices as word processed documents, and handled as
attachments may in the near future be delivered as structured,
processable clinical messages. GP system suppliers would normally adapt
their systems to facilitate the appropriate handling process, advising
practices of any need to change procedures.

++
| > Common examples of attached documents:                              |
|                                                                       |
| -   *Clinical photographs e.g. skin lesions / retinal scans*         |
|                                                                       |
| -   *Scanned images from paper*                                      |
|                                                                       |
| -   *Images from diagnostic equipment*                               |
|                                                                       |
| -   *ECG, Ultrasound scanners*                                       |
|                                                                       |
| -   *Clinical communications (e.g. discharge letters, outpatient      |
|     clinic letters)*                                                 |
|                                                                       |
| -   *Word-processed Documents, Email*                                 |
|                                                                       |
| -   *External hyperlinks -- where the document is not stored locally* |
|                                                                       |
| -   *Numeric results e.g. PEFR reports*                               |
++

### 10.2.1 Legal status

Any attachment to an electronic clinical record should be regarded as
having equal medico-legal weight as a note made within the system and
should be accorded the same stringencies around audit trail and backup
(see chapter 3 'Records Governance'). It should also be possible to
extract these attachments and send them to the requesting practice
either electronically or as a printout.

Before making use of attachment facilities, a practice should satisfy
itself that the system does meet these requirements. Wherever possible
all attached data should be stored on the clinical server and not on a
separate server. If a separate server is used to store attached data,
the practice must ensure adequate and appropriate backup provision to
ensure seamless continuity should failure occur on either clinical or
attachment serving system.

### 10.3 Format of attachments

Potentially a very wide range of document types and formats may be
received or used. Although almost any type of file is viewable with the
correct software, when scanning, practices should generally adhere to a
smaller subset of standard document types as suggested in Table 10.3.1.
This avoids the difficulty of viewing unusual or proprietary formats if
the appropriate software becomes unavailable, particularly where the
records are transferred to another practice.

**Key principles of attachment handling;**

- *Following attachment, any changes made to an editable document must
    be logged in the clinical system's audit trail.*

- *Care must be taken that the document can be faithfully viewed after
    attachment, particularly when documents are scanned. Unusual or
    proprietary formats should be avoided when scanning.*

- *Where a document with an unusual format is delivered to the
    practice, the practice must ensure that appropriate viewing software
    is available and that the type of software required is documented
    within the patient record.*

- *Picture, image files and especially video files can take up
    considerable storage space which should be considered when deciding
    if some types of attachment should be stored in the patient record.*

- *Some formats, particularly JPEG, may result in the loss of image
    detail and should be avoided where the image needs to be of
    diagnostic quality. This may become a particular issue if the image
    is opened and re-saved repeatedly.*

- *When paper documents are scanned, practices should take care to
    make and save a close facsimile of the original document, retaining
    colour information where it is important to do so (e.g. highlighted
    information in a letter). Some image formats such as JPEG, compress
    the data, losing some image quality in the process, so that the
    scanned image may not be an adequate facsimile. Image formats such
    as TIFF and PNG, which do not 'lose information' in this way are
    generally preferable for scanned images.*

- *When scanning a multi-page document, which it is important to
    maintain as a single entity for medico-legal purposes, the TIFF
    format is generally preferred. TIFF can store a number of
    images/pages in a single file whereas JPEG, in its standard form,
    can only store a single image per file and, therefore, a multi-page
    document stored in JPEG format will consist of a number of separate
    files.*

- *Optical Character Recognition (OCR), which attempts to convert
    images of type-written text to word-processable formats, is becoming
    increasingly accurate, sometimes allowing additional semi-automatic
    processing of document headers. However the accuracy of OCR remains
    variable and results of the conversion should be checked carefully.
    Safest practice is always to retain an accurate scanned facsimile of
    the original document.*

- *It is possible to password protect some documents, such that the
    document cannot be viewed without the password. Whilst this may seem
    an attractive means of adding a layer of privacy to particularly
    sensitive documents, in practice it can be very difficult to ensure
    that knowledge of the password can be transferred safely and
    correctly between practitioners. This can result in documents being
    'locked' if the password has become lost through changes of staff
    personnel or transfer to another practice. In general the use of
    per-document passwords should be discouraged and other means should
    be explored for protecting sensitive attachments. Use of native GP
    system or document management system security and privacy facilities
    may be helpful, though this may itself cause problems when
    transferring records to another practice, and ultimately the
    simplest solution may be to retain highly sensitive documents in a
    traditional paper 'sealed envelope'.*

- *NHS England Choose and Book recommends PDF file format for all
    written text, where practically possible.*

### Table 10.3.1

++++
| **Attachment**        | **File formats**      | **Notes**             |
+=======================+=======================+=======================+
| Word-processed        | Microsoft Word 97     | These are editable    |
| documents             | -2010 (DOC, DOCX)     | documents -any        |
|                       |                       | changes made after    |
|                       |                       | attachment must be    |
|                       |                       | represented in the    |
|                       |                       | clinical system's     |
|                       |                       | audit trail.          |
++++
|                       | Open Office (ODT)     | Less common           |
|                       |                       | alternatives to the   |
|                       |                       | MS Word formats.      |
|                       |                       | Audit trail comments  |
|                       |                       | as above              |
++++
|                       | Adobe Acrobat 4 or    | Audit trail comments  |
|                       | higher (PDF)          | as above. Use of the  |
|                       |                       | ability to lock the   |
|                       |                       | document, control     |
|                       |                       | comments and printing |
|                       |                       | should be considered. |
++++
|                       | Rich Text Format      | Audit trail comments  |
|                       | Version 1.5 and above | as above. For         |
|                       | (RTF)                 | compatibility with    |
|                       |                       | non-Microsoft viewers |
|                       |                       | images and graphics   |
|                       |                       | should not be         |
|                       |                       | embedded. Complex     |
|                       |                       | layouts may also not  |
|                       |                       | be retained           |
++++
| Clinical Photography  | Tag Image File Format | This is an old but    |
|                       | v6 (TIFF)             | well tested and       |
|                       |                       | legally admissible    |
|                       | [http://partners.adob | file format that will |
|                       | e.com/public/develope | handle colour and     |
|                       | r/tiff/index.html](ht | black and white       |
|                       | tp://partners.adobe.c | images. It is         |
|                       | om/public/developer/t | difficult to edit but |
|                       | iff/index.html%20)    | still must be covered |
|                       |                       | by the audit trail of |
|                       |                       | the clinical system.  |
|                       |                       | Care should be taken  |
|                       |                       | if the TIFF file is   |
|                       |                       | compressed as not all |
|                       |                       | viewers will handle   |
|                       |                       | compression.          |
|                       |                       |                       |
|                       |                       | Audit trail comments  |
|                       |                       | as above              |
++++
|                       | Joint Photographic    | A popular standard    |
|                       | Experts Group         | supported by the web. |
|                       |                       | The format specifies  |
|                       | (JPEG, JPG)           | compression and a     |
|                       |                       | loss of original data |
|                       |                       | quality. It works     |
|                       |                       | well with natural     |
|                       |                       | pictures and less     |
|                       |                       | well with line        |
|                       |                       | drawings              |
|                       |                       |                       |
|                       |                       | Audit trail comments  |
|                       |                       | as above              |
++++
|                       | Portable Network      | A relatively new      |
|                       | Graphics (PNG)        | standard supported by |
|                       |                       | the web. The format   |
|                       | <<http://www.w3.org/TR> | specifies a           |
|                       | /PNG/>                | compression method    |
|                       |                       | but which avoids a    |
|                       |                       | loss of original data |
|                       |                       | quality               |
++++
| Scanned Images        | Tag Image File Format | For documents for     |
|                       | v6(TIFF), PNG or JPEG | which monochrome      |
|                       |                       | representation is     |
|                       | Resolution of         | sufficient, use TIFF  |
|                       | 150x150dpi is         | with compression      |
|                       | suitable for document | scheme 4              |
|                       | archiving but not for | (COMPRESSION\_CCITTFA |
|                       | diagnostic images.    | X4)                   |
|                       |                       | at a minimum          |
|                       |                       | resolution of         |
|                       |                       | 150x150dpi.           |
|                       |                       |                       |
|                       |                       | For documents that    |
|                       |                       | need to be rendered   |
|                       |                       | with the original     |
|                       |                       | colour information,   |
|                       |                       | JPEG is recommended   |
|                       |                       | with a minimum        |
|                       |                       | resolution of         |
|                       |                       | 150x150dpi and a      |
|                       |                       | compression quality   |
|                       |                       | \>=50%                |
|                       |                       |                       |
|                       |                       | Audit trail comments  |
|                       |                       | as above.             |
|                       |                       |                       |
|                       |                       | Data loss comments    |
|                       |                       | due to compression as |
|                       |                       | above.                |
++++
| Images from           | Proprietary           | Wherever possible     |
| diagnostic equipment  |                       | proprietary formats   |
|                       |                       | should be avoided for |
|                       |                       | reasons of future     |
|                       |                       | legibility. Where     |
|                       |                       | this is not possible, |
|                       |                       | clear directions and  |
|                       |                       | reasons for recording |
|                       |                       | in this way should be |
|                       |                       | retained along with a |
|                       |                       | CD containing the     |
|                       |                       | viewing software.     |
++++
|                       | JPEG, PNG, TIFF       | Still image -- As     |
|                       |                       | above for clinical    |
|                       |                       | photography           |
++++
|                       | High Quality          | Most modern X-ray and |
|                       | Diagnostic images     | Ultrasound devices    |
|                       |                       | will produce high     |
|                       |                       | diagnostic quality    |
|                       |                       | (still or moving)     |
|                       |                       | images. They are      |
|                       |                       | generally out of the  |
|                       |                       | scope of this         |
|                       |                       | document but          |
|                       |                       | potential users in    |
|                       |                       | General Practice      |
|                       |                       | should satisfy        |
|                       |                       | themselves that the   |
|                       |                       | system's storage      |
|                       |                       | conforms to the       |
|                       |                       | clinical system's     |
|                       |                       | audit trail           |
|                       |                       | requirements as well  |
|                       |                       | as published          |
|                       |                       | standards such as     |
|                       |                       | DICOM                 |
|                       |                       | (<http://medical.nema>. |
|                       |                       | org)                  |
++++
|                       | AVI, QuickTime,       | Moving images         |
|                       | MPEG2, MP4            |                       |
|                       |                       | These are all popular |
|                       |                       | methods of delivering |
|                       |                       | moving information.   |
|                       |                       | Both may involve      |
|                       |                       | significant           |
|                       |                       | compression and data  |
|                       |                       | loss and should be    |
|                       |                       | used for thumbnail    |
|                       |                       | and aide-memoire      |
|                       |                       | purposes. They should |
|                       |                       | not be generally used |
|                       |                       | for diagnostic        |
|                       |                       | purposes.             |
++++
| Email                 | Plain text            | Preferred over HTML   |
++++
|                       | HTML                  | Should not include    |
|                       |                       | external references,  |
|                       |                       | hyperlinks,           |
|                       |                       | backgrounds or fonts  |
|                       |                       | which may not be      |
|                       |                       | available on other    |
|                       |                       | systems               |
++++
| External hyperlinks   | http://\<resource     | The resource should   |
|                       | URL\>                 | be available to all   |
|                       |                       | potential users of    |
|                       | ftp://\<resource      | the clinical record   |
|                       | URL\>                 | and should not link   |
|                       |                       | to resources only     |
|                       |                       | available at the      |
|                       |                       | practice. Commitment  |
|                       |                       | to the continued      |
|                       |                       | maintenance and       |
|                       |                       | backup of these       |
|                       |                       | resources must be     |
|                       |                       | assured.              |
++++

### 10.4 Storage of attachments

GP systems store attached documents in a variety of ways, and generally
provide guidance and user training material on best practise for storing
attachments. These instructions should be understood and carefully
complied with by practice staff.

In some cases, attachments are simply saved to a specific area on the
practice network; in others the attachments are stored directly within
the patient record database. A 'Document management package' may be used
along with either of the previous options, generally adding more
sophisticated handling or 'workflow', of incoming documents, along with
detailed document categorisation and labelling facilities. Most Scottish
practices now use the NHS Scotland approved 'Docman' package.

Whatever combination of approaches is employed, the practice must ensure
that the attachments are treated exactly as other patient records, are
backed up securely, are available for transfer to another practice, and
are accessible to patients under terms of the Data Protection Act.

### 10.5 Attachment identification and coding

When attaching a clinical document, it is important to name or
categorise the document within the local GP system so that its source
and clinical significance is readily apparent when the patient record is
subsequently viewed, without needing to open the document itself. The
attachment should also be correctly attributed and coded to facilitate
querying.

### 10.5.1 Attribution

As with any clinical record it is vital that the attribution of the
attachment is captured so that date, time and where appropriate
clinician or operator are available as well as the date and time and
operator making the attachment.

### 10.5.2 Coding of numerical contents

Where a document includes significant numeric data and several values
are derived together (Lung Function testing may derive Peak Flow, FEV1,
FVC etc.), each value should be stored against an appropriately coded
entry to facilitate system functionality and subsequent retrieval.

### 10.5.3 Attachment identification

If an attachment needs to be subsequently identified or 'labelled'
within a patient record, a meaningful description such as ***\'Discharge
letter Cardiology Western Infirmary Anytown\'*** is clearly more
informative to the viewing clinician than a bland label such as ***'File
Attachment'***, and which would require the document to be opened to
ascertain its contents.

Work is progressing at UK level to define standard ways of labelling
clinical documents across a wide range of care settings, but at present
no such standard has been agreed, other than for Scottish GP practices,
which store attached documents within a common set of 'Docman' folders,
primarily based on speciality type[^1]:

A UK-wide clinical document identification standard is likely to include
the following elements which offer a minimal but effective way of
communicating the contents of a clinical document (see table 10.5.3)

### Table 10.5.3

  **Label element**    **Examples**

  **Document type**   "Clinic letter", "Discharge document"
  **Speciality**      "Occupational therapy", "General medicine"

This approach, coupled with the use of standard lists of document types
and speciality names may, in time, lead to the majority of NHS clinical
documents being labelled 'at source', substantially reducing the need to
do so within GP practices or any other document recipient.

The method of applying a label or category to the attached document will
depend on the GP system used and whether a document management package
or other formal categorisation facility is available. Use of such formal
categorisation is the recommended approach, wherever possible. Most
document management packages allow attached documents to be categorised
in a variety of ways, which it would normally be possible to adapt to
use the recommended Document type and Speciality categories.

Where formal document categorisation facilities are not available, it
may be helpful to use the suggested elements to construct a single label
or description for the attachment

e.g. "***Discharge document General Medicine***"

If the system does not allow a description to be recorded for an
attachment, it may be helpful to construct the saved file name in a
similar fashion.

e.g. ***"Discharge document General Medicine.doc"***

When creating file names, it is generally best to avoid using any
punctuation marks other than the dot character, as these may not be
uniformly acceptable across all computer operating systems.

**Choose & Book referral attachment names**

Choose & Book guidance suggests naming attachments with recognisable
filenames such as:

**Surname, forename, date of birth** e.g*. **johnsmith23061966*** as a
basis for ensuring files are easily recognisable and associated with
specific patient records.

### 10.6 Transferring attachments

A common issue arises when patients leave a practice and their records
require to be transferred to the new practice or other agency.

### 10.6.1 Legal issues

When a patient moves to a different practice, it is legally incumbent
upon the original practice to respond to a request to transfer the
patient's whole medical record. The legal requirement is that either
party may insist on the records being transferred as paper printouts,
and of course, in many practices, significant parts of the clinical
record will still be available only in paper format. However, when some
or all of the clinical record is held in electronic form, the use of
some means of electronic transfer of the record is much less
time-consuming for both practices, particularly for attached documents
which otherwise have to be printed out by the original practice, then
re-scanned by the recipient practice (see Chapter 9.7.8).

### 10.6.2 Modes of transfer

Within the UK four nations, there are currently significant differences
in approaches to the electronic transfer of GP clinical records,
including the transfer of attached documents:

### 10.6.2a NHS England

**10.6.2a.1 GP2GP records transfer**

When available, the NHS Connecting for Health GP2GP project offers the
most safe and practical means of effecting electronic transfer of
records between practices. It incorporates the transfer of electronic
attachments (with the limitation of a maximum of 100 attachments and a
5MB limit per patient record), generating an attachment file-manifest,
which associates attachments with a patient record irrespective of the
filename. ***See Chapter 8b - Data transfer & inter-operability, for
guidance on GP2GP records transfer.***

**10.6.2a.2 CD-ROM based attachment transfer**

Although GP2GP rollout continues to progress in England (and is the
professionally preferred method of electronic record exchange) it is not
yet available for all GP systems. As an interim step, an alternative
means of transferring attached documents via CD-ROM disc has been
developed by an IM&T Committee consisting of members of the Beds and
Herts. Local Medical Committee, GPs, practice staff and PCT staff,
working in cooperation with several GP system suppliers.

Detailed guidance on operating this CD-based transfer, including advice
from individual GP system suppliers, is available from the project
website[^2].

The protocol has been operating successfully in a number of PCTs, to the
benefit of both sending and receiving practices but the following
principles and caveats should be noted;

- *Formal permission should be sought from the Sending practice's PCO
    to allow CD-based transfer.*

- *The process should not be carried out until administrative staff
    have received training in the necessary procedures, as documented at
    the project website, both to create the outgoing CD and to import
    attachments from the received CD.*

- *The procedures advised by the appropriate GP system supplier should
    be closely followed to prevent potential loss of information in the
    transfer process.*

- *The recipient practice retains the right to receive the record and
    attachments in paper format if they so desire, but must request this
    from the sending practice in a timely fashion.*

- *Only non-rewriteable CD-based transfers are acceptable. Other media
    such as DVD, floppy discs and USB memory sticks have significant
    risks and drawbacks in comparison.*

- *After importing and checking the data, the CD received must be
    shredded or destroyed by cutting -- the project website gives
    further instructions.*

**10.6.2a.3 CD encryption issues**

Dept. of Health information guidance suggests that where clinical
documents are electronically transferred outwith the practice, patient
privacy should be protected by the use of encryption and passwords, in
case of inadvertent loss or interception of the document in transit.

> *"David Nicholson, NHS Chief Executive, has directed that there should
> be no*
>
> *transfers of unencrypted person identifiable data held in electronic
> format*
>
> *across the NHS. This is the default position to ensure that patient
> and staff*
>
> *personal data are protected. Any data stored on a PC or other
> removable*
>
> *device in a non secure area or on a portable device such as a laptop,
> PDA or*
>
> *mobile phone should also be encrypted. This is also now a
> requirement*
>
> *across all public sector organisations set by the Cabinet Secretary.*
>
> *It is recognised however that this may take some time to achieve in
> the NHS*
>
> *where patient care is our highest priority. NHS bodies will need to
> make a local judgement on the balance of risk to patient care against
> risk to personal*
>
> *data security in determining whether use of unencrypted devices
> should*
>
> *continue as an interim measure. Where it is felt that continued
> reliance upon*
>
> *unencrypted data is necessary for the benefit of patients, the
> outcome of the*
>
> *risk assessment must be reported to the organisation's Board, so that
> the*
>
> *Board is appropriately accountable for the decision to accept data
> vulnerability or to curtail working practices in the interests of data
> security."*[^3]

This is one rationale for the use of approved NHS mail and messaging
facilities such as the Spine and SCI-Gateway, which provide such
security automatically for emailed attachments and clinical messages
such as electronic referrals and GP2GP record transfers.

To comply fully with the DH directive, a CD used for attached document
transfer should be encrypted, but this considerably complicates the
transfer process, requiring agreement on the encryption method,
availability of the appropriate encryption/decryption software in both
practices and communication of the associated password in a secure and
timely fashion. If not handled correctly, it may also interfere with
patient rights to access records under the Data Protection Act.

In view of such added complexity, the CD transfer project team judged
that within this very specific context, encryption adds little to
patient privacy protection, given that the CD-ROM is physically
transferred via a secure courier service alongside a set of unencrypted
paper printouts of other aspects of the clinical record.

Whilst generally acceptable to participating practices, PCOs and
suppliers, this advice has not been formally endorsed by practitioner
representative bodies, NHS, or medical defence advisers. It remains
likely that in due course formal guidance will be introduced, jointly
with the Dept. of Health, on standard methods of encryption of CD-based
document transfers and associated operating procedures.

Until such time, where encryption is not used, practices should make an
individual assessment of the risk of a privacy breach and agree the
approach with their PCO.

Full DH Information Security Guidance may be found on their website[^4]

### 10.6.2b NHS Scotland

**10.6.2b.1 Docman Transfer**

Almost all Scottish GP practices now use the 'Docman' document
management package and associated standardised folder structure. The NHS
Scotland Practitioner Services 'Docman Transfer' facility allows the
automated transfer of attached documents between practices without the
need for the documents to be re-filed in the recipient practice. In
addition, an export of the entire GP system patient record to an
electronic document may be made, imported to Docman and transferred
electronically with the other attachments.

At publication, the 'Docman Transfer' facility was available to 95% of
Scottish practices and for these practices represents the simplest and
safest approach to attached document transfer. Details of the 'Docman
Transfer' process are available online[^5]

**10.6.2b.2 CD-ROM based attachment transfer**

The use of compact discs (CDs) to exchange attachments or other
electronic records is not currently formally supported by the NHS in
Scotland. Any such arrangement would be strongly discouraged where
'Docman Transfer' is available but if necessary it should be agreed on a
per-case basis between sending and receiving practices. The protocol
used within NHS England for CD-ROM attachment transfer (see above) may
be regarded as a robust model on which to base any local arrangement.

**10.6.2b.3 GP2GP records transfer**

NHS Scotland is examining the possibility of making GP2GP records
transfer available. In these circumstances, GP2GP is likely to offer the
most safe and effective means of electronic transfer of records
(including attached documents).

### 10.6.2c NHS Wales

**10.6.2c.1 GP2GP records transfer**

NHS Wales have indicated that GP2GP records transfer will be made
available as part of National Programme, led by the NHS Wales
Informatics Service (GMS IM&T Programme). When it becomes available, it
will offer, to Welsh practices, the most safe and practical means of
effecting electronic transfer of records (including attached documents).

**10.6.2c.2 CD-ROM based attachment transfer**

The use of compact discs (CDs) to exchange attachments or other
electronic records is not currently formally supported by the NHS Wales.
Any CD based transfer would have to be agreed on a per-case basis
between sending and receiving practices and seeking prior clearance from
a PCO. CDs must be encrypted and transferred via the all Wales secure
courier service. The protocol used within NHS England for CD-ROM
attachment transfer (see above) could be adapted to provide a model on
which to base any local arrangement.

### 10.6.2d HSC N. Ireland

**10.6.2d.1 GP2GP records transfer**

At the time of writing (July 2010) we have no information on GP2GP
records transfer in Northern Ireland.

**10.6.2d.2 CD-ROM based attachment transfer**

The use of compact discs (CDs) to exchange attachments or other
electronic records is not currently formally supported by the Health and
Social Care organisations in Northern Ireland. Any CD based transfer
would have to be agreed on a per-case basis by the Health and Social
Care organisations and between sending and receiving practices. The
protocol used within NHS England for CD-ROM attachment transfer (see
above) may be regarded as a robust model on which to base any local
arrangement.

### 10.7 e-referral attachments

Chapter 9 outlines the use of e-Referral systems (section 9.7.9). Both
of the main e-referral packages in use, Choose & Book and SCI Gateway,
allow the upload of attachments along with the referral e.g. a scanned
document or clinical image. Most of the common file formats listed in
Table 9.2.1 are supported but there may be some minor limitations along
with restrictions on numbers of attachments and attachment size per
referral. These limitations are unlikely to be significant in usual
practice and relevant system documentation should be consulted for
specific guidance.

### 10.7.1 Choose and Book attachment limitations

It is not possible to add notes or letters from a GP system directly
into a Choose and Book 'Advice and Guidance' request. Instead you should
copy / paste from a practice system into the body of the advice request
or save the additional information in a document outside of the practice
system and then add it as an attachment.

###

### 10.8 Other documents

Practices maintain many different forms and documents about patients
that are essential to their day to day operations. Some of these do not
form part of the patients' records but carry information about patients,
carers and others. Below, we give some examples of these documents and
advice about their retention and disposal;

- *Notification of infectious disease -- no need to retain counterfoil
    providing there is an appropriate entry in the relevant EPR. In NHS
    Scotland, notifications are performed electronically via SCI
    Gateway.*

- *Message books/logs -- ensure any action taken (e.g. phone
    call/consultation/visit) is recorded in the EPR. It is advisable to
    retain written message books/logs in line with general medico-legal
    guidance.*

- *Ambulance request logs -- ensure any action taken is recorded (as
    above)*

- *X-ray films. These should be retained in line with the DoH guidance
    above (see Chapter 3).*

Most of the above are "process" forms but may be important
medico-legally. If practices are in any doubt about retaining a document
we recommend that they scan and store an image of the document in an
appropriate format (see Table 10.3.1) and then shred the original
document. However, where any records relate to patients where there are
known medico-legal issues (complaints, civil or criminal law) then
practices should keep all relevant records pending further advice from
their medical defence organisation, PCO or LMC.

[^1]: [http://www.scimp.scot.nhs.uk/\.../Procedures%20%20DocMan%20Document%20Folders%20v2.3.doc](http://www.scimp.scot.nhs.uk/.../Procedures%20-%20DocMan%20Document%20Folders%20v2.3.doc).

[^2]: [http://www.starpace.co.uk/page.asp?pageID=97](http://www.starpace.co.uk/page.asp?pageID=97%20)

[^3]: <http://www.connectingforhealth.nhs.uk/systemsandservices/infogov/security/encryptionguide.pdf>

[^4]: [http://www.dh.gov.uk/prod\_consum\_dh/groups/dh\_digitalassets/\@dh/\@en/documents/digitalasset/dh\_074141.pdf](http://www.dh.gov.uk/prod_consum_dh/groups/dh_digitalassets/@dh/@en/documents/digitalasset/dh_074141.pdf%20)

[^5]: [http://www.psd.scot.nhs.uk/professionals/medical/DocmanTransfer.html](http://www.psd.scot.nhs.uk/professionals/medical/DocmanTransfer.html%20)
