---
title: 7. Clinical Coding Schemes
---

# 7. Clinical Coding Schemes

### 7.1 Coding Schemes in Current Use

![](media/image1.jpeg){width="2.998611111111111in"
height="1.9in"}Electronic records in General Practice have had coding
schemes at their heart since the 1980s, in some cases even earlier. More
than 520 million separate coded entries were added to England's EPRs in
2006. This is approximately double the volume of ten years ago, and the
year-on-year trend is clearly for even more coded data (see graph) [^1].

In the 1980s, personal computer schemes were in their infancy, and had
(by today's standards) tiny memories both in terms of computer RAM and
disc storage. Two of the earliest clinical classification or coding
schemes developed specifically for computers were OXMIS (now effectively
obsolete) and the READ codes developed by Dr James Read, a GP in
Loughborough.

The principal reason for "coding" at that time was to reduce the memory
required to store patient records by replacing the full-text description
of commonly recorded clinical concepts (described in English by a "term"
(an English word or phrase)) with short codes (typically 4 or 5
alpha-numeric characters). A second important feature of coded concepts
in practice was that only a few characters needed to be typed for the
complete text of matching clinical concept descriptions to appear on the
screen for selection. Thus, clinicians didn't need to become proficient
in typing entire descriptions, and so records could be created more
quickly - even during the consultation - and with fewer typing mistooks.

In 1987, the Joint Computing Group of the RCGP and GMSC adopted the then
named *Read Clinical Classification* as the standard coding scheme for
GP records in the UK[^2].

### 7.2 Future standardisation of coding schemes across health care. SNOMED-CT

At the time of writing this chapter in 2010, there is the imminent
prospect that the NHS scheme of coding will migrate to the new NHS
standard, SNOMED-CT (SNOMED Clinical Terms) over the next 2-5 years.
SNOMED-CT is a terminology which is the result of the merger of 2
competing terminologies at the end of the 1990s, SNOMED-RT -
Systematised Nomenclature of MEDicine Reference Terminology, (from the
College of American Pathologists in the USA), and CTV3 - Clinical Terms
Version 3 (from the UK, and at the time of merger in 1999 the
responsibility of the NHS Information Authority). CTV3 is the direct
descendent of Read Version 2 (RV2 -- see below): it contains the same
content (and more) but delivered in a technically different (and better)
way. The merged product, SNOMED CT, is therefore also a descendent of
RV2 and so has the same content, and more besides.

The real benefits of Snomed-CT implementation, in allowing all health
sectors to communicate and share data more reliably will only come when
it is the native coding scheme for all clinical systems.

### 7.3 Features of Read Codes

Read codes are the predominantly used coding scheme in General Practice
at the time of writing this chapter (June 2010). There are now only
really two official flavours of the Read codes: the Scottish and English
releases. These differ only in certain aspects of the codes and terms
available within Chapter 9 (administrative codes). Practice- or
supplier-specific local codes have created hundreds of subflavours (see
7.4.6).

### 7.3.1 4 Byte Read, (Read version 0)

The original 4-Byte Read codes are now no longer maintained or released,
and so are now obsolete. As implied in the name, this terminology used
four characters in each code. Each code uniquely identifies the term or
concept, and also fixes the term in relation to other terms in the
scheme.

Allowable characters in the code include A-Z, a-z, 0-9, with the
exception of i, o, I, O, i.e. a total of 58 options.

In the 4-byte set this gives a total of 58^4^ or 11,316,496 possible
unique concepts, though in practice fewer than 90,000 were ever used.
Synonyms were also provided for in the 4-byte set, but although this
allowed increased breadth of expression for clinicians, there was no
means of identifying a synonym uniquely other than with the free text
string recorded. By 2009, no known 'live' systems still used this
terminology and it was discontinued. However, many live systems will
contain records that include some data originally entered on a 4-Byte
READ system (typically, during the 1990s or earlier). By now, this
legacy data may have been moved several times between different systems.
It is known that some of the early migrations - in particular those from
4-Byte Read Codes - were not always accurate.

### 7.3.2 Read codes Version 2 (RV2 - also known as the 5 byte, or unified set)

The 5-Byte Read scheme (RV2) is the most commonly used version of the
Read codes in UK systems. In this version, which became known as the
5-byte or 'unified' set, an extra character was added to the code to
increase the possible number of different codes up to 58^5^ or
656,356,768.

Whilst 656,356,768 maybe the theoretical maximum number of symbols,
because of RV2's strong hierarchical structure and the way that
structure is represented within the codes themselves, it isn't
necessarily the case that we could actually fit and properly organize
that many clinical concepts within RV2. Certain sub-hierarchies are
already demonstrably 'full' and/or no longer properly organized.

They are revised by the UK Terminology Centre (UKTC) every six months
(monthly for the RV2 drug dictionary). The total number of codes in RV2
today (the October 2010 release) is 94,937 and the current rate of
growth is approximately 1200 new codes per annum. However, 98.85% of all
new additions to the primary care record are typically expressed using
codes from a set of just 10,000 commonly used codes, although the
membership of this set drifts over time.

From a technical perspective, RV2 has many more similarities than
differences with the pre-existing classifications, particularly ICD-9
and OPCS. Not only do all three arrange their codes in 'chapters', but
RV2's particular chapter organization and content for the Diagnoses
chapters (A-V) deliberately mirrors that of ICD-9 and 10 very closely,
to facilitate the mapping between them. Chapter 7 of RV2 (Procedures) is
similarly very close to OPCS-4.5.

The important differences are therefore primarily in RV2's extra content
not found in either ICD or OPCS, including for example, the drug,
administrative, sign and symptom codes, and the occupation code chapter
0 (although, empirically, not all of these additions are actively or
reliably used today in UK primary care).

### 7.3.2.1 Chapters in 5-Byte Read (RV2)

RV2 codes are arranged in chapters. Diagnoses are arranged in chapters A
through to V, (excluding I and O, which do not exist), and other
categories of code are in chapters 0-9

The chapter headings in RV2 are:

> A. Infectious/parasitic diseases\
> B. Neoplasms\
> C. Endocrine, nutritional, metabolic, and immunological diseases\
> D. Blood/blood forming organs diseases\
> E. Mental disorders\
> F. Nervous system/sense organ diseases\
> G. Circulatory system diseases\
> H. Respiratory system diseases\
> J. Digestive system diseases\
> K. Genitourinary system diseases\
> L. Pregnancy, childbirth, and puerperium\
> M. Skin and subcutaneous tissue diseases\
> N. Musculoskeletal and connective tissue diseases\
> P. Congenital anomalies\
> Q. Perinatal conditions\
> R. Symptoms, signs, ill defined conditions[^3]\
> S. Injury and poisoning\
> T. Causes of Injury and poisoning\
> U. External causes of morbidity and mortality\
> V. Unspecified conditions.

And the other chapters are:

0\. Occupations\
1. History and symptoms\
2. Examination and Signs\
3. Diagnostic procedures\
4. Laboratory procedures\
5. Radiology/physics in medicine\
6. Preventative Procedures\
7. Operations, procedures, sites\
8. Other therapeutic procedures\
9. Administration.

### 7.3.2.2 The 5-Byte Read Hierarchy

One of the most powerful features of many clinical classifications and
terminologies, including the 4- and 5-Byte Read Codes, is the structure
using hierarchies. RV2 organises its coded clinical concepts into a
hierarchy, thus allowing both primary encoding of conditions at
different levels of detail *and* the ability to later retrieve coded
information from the electronic record's database using this
hierarchical structure. The hierarchy of Read is known as a *typology*,
or *"is a"* ("is a type of") hierarchy. See Example 1.

![](media/image2.png){width="2.6972222222222224in" height="4.0in"}Each
RV2 code represents a term or short phrase describing a health-related
concept. For example, in the Respiratory diseases chapter we can see a
hierarchy for asthma:

+-----------+-----------+------------------------------------------+
| Hierarchy | Read Code | Term                                     |
|           |           |                                          |
| level     |           |                                          |
+===========+===========+==========================================+
| 1         | H         | Respiratory system diseases              |
+-----------+-----------+------------------------------------------+
| 2         | H3        | Chronic obstructive pulmonary disease    |
+-----------+-----------+------------------------------------------+
| 3         | H33       | Asthma                                   |
+-----------+-----------+------------------------------------------+
| 4         | H331      | Intrinsic asthma                         |
+-----------+-----------+------------------------------------------+
| 5         | H3311     | Intrinsic asthma with status asthmaticus |
+-----------+-----------+------------------------------------------+

In this example from the 5-byte GP set, it can be seen that data is more
and more detailed at each successive hierarchical level. This
tree-branching hierarchical structure enables the clinician to have not
only the ability to encode his/her patient\'s clinical data in detail
(or not), but also to later collect information from the target
population of the practice, by searching for codes at more general
levels of detail. He/she can ask his computer system to search at level
1 to find all the respiratory diseases recorded in the database, level 2
to find all cases of COPD, level 3 at a more specific level (asthma),
and so on. Much more sophisticated searches can be performed. Notice the
dual function of the code-for both unique concept representation, and
fixing the concept\'s position in the hierarchy.

While this represents an "ideal" view of hierarchies and the functions
they might support, in practice things are inevitably more complex. For
example, retrieving all patients with a code beginning 'A1' -- ie all
hierarchical descendents of \[A1\... Tuberculosis\] from the infectious
diseases chapter - will NOT reliably give you everybody with TB:

-   Late effects of TB are under AE0..

-   TB of bone is duplicated under N306, N305 and N304.

-   Congenital TB is Q4024

-   Various organ specific sequelae of TB are distributed all over the
    place.

In practice, almost all patients with a code indicating TB infection are
actually coded directly to A1... itself, but a smattering of 1411.,
65Y9., 65V9. and N304. encodings exist to be missed by the unwary. The
phenomenon is encountered in many general clinical queries.

### 7.3.2.3 Terms in 5-Byte Read (RV2)

Like 4-Byte READ, RV2 allows the use of both preferred terms and
synonyms (different terms with equivalent meaning e.g. *myocardial
infarction* (preferred term) and "*heart attack*" (synonym)). RV2 allows
rapid look up of commonly used terms, using keys and partial text
strings.

\(i) indexed keys (also called abbreviations). Commonly used terms are
indexed by a "key" which may be up to 10 characters long.

\(ii) Some systems allow the user to look up concepts using only the
beginning of words in the complete term (e.g. "myoc inf" would retrieve
38 codes relating to *myocardial infarction* plus one relating to *acute
myocarditis - influenzal ).* This functionality is system specific and
so try to find out from colleagues how look-ups are optimised on your
practice system.

Word equivalence tables can be used with any terminology, so that common
variant or misspellings may still find the term searched for (e.g.
foetus - fetus, cancer -- malignancy, tumour -- mass). Although a
standard (but incomplete) set of keys and word equivalents are published
by the UK Terminology Centre with the RV2 release, most system suppliers
use their own sets instead but these are all slightly different, giving
different results for users' search strategies on different systems
(locums beware!). In addition, suppliers may also allow customising of
keys at each site, which can help individual practices code consistently
but will be a further obstacle to NHS wide uniformity.

The design parameters for 4-byte Read set a limit of 30 characters of
text for any term to describe a concept. This enabled all 4-Byte Read
terms to be displayed over two columns on the 80-character-wide computer
displays of the day. This (at times challenging) limit was increased in
RV2, such that an option of a 60 and/or 198 character spelling variant
*of the same term* was also allowed. (This extended file structure was
developed in 1991, and is known as the Version 2 file structure.)

> **Example of 30-, 60- and 198-Character term variants of the same
> term**
>
> Read Code:38Du1 Term Code:00
>
> Term30: IAPT phob sc - Cer si fr pa di
>
> Term60: IAPT phobia scale - Cert situ fear panic attak distres symp
>
> Term198: Improving Access to Psychological Therapies programme phobia
> scale - Certain situations because of a fear of having a panic attack
> or other distressing symptoms

Additionally, in RV2, a clinical idea or concept coded by a Read Code
can also be expressed by more than one term (synonyms). One of these is
designated the "preferred term", and given a 2-digit "term code" value
of "00". Further synonyms are represented with 2-character term codes.
These are [normally]{.underline} numeric and in the range 11 -- 99[^4]
(example 2), though a minority of term codes are alphanumeric (1A, 1B
etc). This enables the exact term (preferred or synonym) which the
clinician intended to record to be persistently stored, retrieved or
transmitted intact, thus preserving the language used at the point of
patient contact. A concept, expressed in the language actually chosen by
the clinician at the point of patient care, is thus most properly
expressed as the Read Code [plus]{.underline} the term code (i.e. 7
characters in all, not 5). This is especially true because of the
'pseudo-synonym' problem described below.

Although RV2's synonym encoding would have been workable in theory, in
reality significant errors have crept into the RV2 release data
concerning synonyms. Broadly, two problems will be encountered:

1.  Pseudo-synonyms -- terms that are not true synonyms

Casual scrutiny of RV2 will reveal many instances of synonyms of
preferred terms, which are not actually true synonyms. In the examples
below, the code G30.. combined with the term code 13 does not mean the
acute event of a heart attack, but rather a condition that may occur at
some interval after the original heart attack. None of the different
term codes for N245. are synonyms of each other.
![](media/image3.wmf){width="5.739166666666667in"
height="2.7989938757655293in"}

The UKTC has determined that at least 3.7% of all RV2 5-Character codes
have at least one non-synonymous term, but also that the phenomenon is
relatively concentrated in that portion of the RV2 code-set most
actively used by GPs: of the top 10,000 codes by use (collectively
accounting for 99% of the EPR), at least 11.3% have at least one
non-synonymous term. 27% of these are cases of commonly used V2 synonyms
but that properly have a different meaning to the preferred term for the
same 5-character V2 code. Some of the more commonly used RV2 synonyms
that don't mean the same as their preferred term include:

  ------------------------------------------------------------------------------
  CODE/TERM CODE COMMONLY USED...     ...DOES NOT MEAN THE SAME AS
  ----------------------------------- ------------------------------------------
  662.. 12 Hypertension monitoring\   662.. 00 Cardiac disease monitoring\
  N245. 17 Shoulder pain\             N245. 00 Pain in limb\
  66C9. 11 Weight loss advised\       66C9. 00 Target weight discussed\
  8H7.. 12 Referral to nurse\         8H7.. 00 Other referral\
  663.. 11 Asthma monitoring\         663.. 00 Respiratory disease monitoring\
  1A\... 12 Urinary symptoms\         1A\... 00 Genitourinary symptoms\
  62\... 11 Antenatal care            62\... 00 Patient pregnant

  ------------------------------------------------------------------------------

Whilst there are mechanisms to try and prevent the loss of meaning and
misreporting for such situations, they are not always successful. It is
therefore worth trying to avoid using "non-synonymous synonyms" whenever
possible.

2.  Duplicates - same term but different code

UKTC has determined that RV2 includes approximately 5700 cases where one
code and term code -pair apparently means the same thing as a completely
different one. Many of these are inherited from ICD, where the same
problem exists when the same clinical concept needed to be in two
different chapters. Others represent authoring errors in RV2.

Some of the pairs more commonly in active use by GPs today include:

+----------------------------+---------------------------------------+
| 1C13. 00 Deafness\         | 66U.. 11 Hormone replacement therapy\ |
| F59.. 11 Deafness          | 8B64. 00 Hormone replacement therapy  |
|                            |                                       |
| 9877\. 11 Injection given\ | N245. 13 Foot pain\                   |
| 85D.. 00 Injection given   | 1M11. 00 Foot pain                    |
+----------------------------+---------------------------------------+

Both the above problems -- pseudo-synonyms and duplicate concepts -
increasingly hamper efforts to extract value from RV2-encoded data.
However, because of other design limitations of RV2, these errors cannot
be corrected within RV2 itself. Part of the fundamental design rationale
for CTV3 was not only to create a terminology free of these errors, but
also one within which it was possible to correct new errors as they
arise in future. The issue remains an important reason why the NHS
recommends replacement of RV2 with a still more sophisticated
alternative (SNOMED-CT).

**Table 7.3.2.4 Abbreviations used in some Read terms**

  *Abbreviations used in some Read terms:*   Meaning                                                     Notes
  ------------------------------------------ ----------------------------------------------------------- -------------------------------------------------------------------------
  NOS                                        Not otherwise specified                                     Classification term from ICD -- *avoid use if possible*
  NEC                                        Not elsewhere classified                                    Classification term from ICD -- *avoid use if possible*
  EC                                         Elsewhere Classified                                        Classification term from ICD -- *avoid use if possible*
  \[D\]                                      a symptom used as a working diagnosis                       Birmingham Research Unit of RCGP. Used in sentinel practice network[^5]
  \[M\]                                      Morphology concepts relating to histology of tumours only   *Use only if encoding morphology from histology results*
  \[SO\]                                     "Site of" intended operation (not symptom of)               *Use should be limited to this category of entry*
  \[V\]                                      From ICD9 "reason for visit" codes                          From ICD classification

### 7.3.3 Clinical Terms Version 3 (CTV3)

Clinical terms version 3 (previously called Read Codes version 3) is now
used by two systems in England: TPP's SystmOne, and HealthySoftware's
Crosscare. The October 2010 release of CTV3 contains 298,102 concept
identifiers, of which 55,829 are retired or extinct and should not be
used (or present in historical records). CTV3 is growing at a rate of
around 6,200 new concept identifiers annually (though many of the new
codes relate to new pharmaceutical products in the READ Drug Dictionary;
the rate of addition of non-drug content is only slightly more than the
1200 added annually to RV2).

CTV3 built upon RV2's clinical content and aimed to incorporate a
comprehensive set of clinical concepts for use across both primary and
secondary care. It was introduced in the mid 1990s after consultation
with over 50 specialist groups across medicine, nursing, midwifery and
allied professions.

Unlike 4- and 5-Byte Read, the dual function of the central 5-character
concept code has been abandoned In CTV3: neither the hierarchical
position of the concept, nor any of the associated terms, is directly
defined by the code. Critically, this enables concepts to have more than
one parent concept, and thus effectively allows a single concept to
appear in more than one part of the hierarchy, but with only one Read
Code. In retrieval of information from the patient database, this has
obvious advantages.

-   *The code becomes only a unique identifier of a concept*

-   *The position of the concept in a hierarchy is not code dependent.
    This is now defined by tables, which list parent -- child concepts
    in a table. Clinical Terms Version 3 contains a hugely increased
    number of concepts, terms and synonyms in comparison to the previous
    Read code schemes above. This is because the CTV3 scheme was
    designed to include a comprehensive set of concepts to cover the
    whole of health care, not just primary care.*

In order to provide backward compatibility, CTV3 is a "superset" of
previous versions of the Read codes, meaning that all previous concepts
and terms exist within CTV3. Mapping tables now exist between Read
4-byte and Read 5- byte, Read 5-byte and CTv-3, Read 5-byte and
SNOMED-CT, and CTV3 and SNOMED-CT.

Clinical concepts are still arranged in a hierarchy. Instead of using
the code, the position is defined in parent-child tables in the Version
3 file structure. This also allows more than five hierarchical levels,
though in practice, nine levels have rarely been exceeded. The hierarchy
which is built up from the parent-child relationship tables is called a
typology, or "is-a" hierarchy, as a \<child concept\> is-a (type of)
\<parent concept. e.g. \<Asthma\> is-a \<Respiratory Disease\>.

CTV3 terms have their own 5-character term code, each of which codes for
a triad of a 30-, 60- and 198-character length variant of the same
descripton (as in RV2). CTV3 term codes all begin with the letter Y or
y.

Content errors can be fixed in CTV3: at each successive 6 monthly
release, UKTC can move codes and terms about within the hierarchy
independently of each other, or withdraw (retire) them from active use
entirely. This flexibility comes at a price, however: previously
captured data -- and previously authored reporting query definitions -
need to be modified each time there is a new CTV3 release, to substitute
instances of retired or otherwise deprecated content with recommended
current replacements. Failure to do this may lead to incorrect querying
behavior (principally, codes that used to be returned in response to
stock queries no longer are, so that some patients are missed). A more
elaborate version of the same functionality is part of SNOMED CT.

**7.3.3.1 Qualifiers, added detail, and clinical terms version 3**

The amount of detail required in a comprehensive thesaurus is
overwhelming, and in order to cope with this, CTV3 adopted a scheme
whereby fine detail may be added to \'core terms\' by adding extra
codes, or \'qualifiers\'. Thus, the complete clinical description is
recorded as a bundle of codes, rather than only one. For example, in
order to encode a 'pain in the *left* ankle' you would record 3 codes:

X75sF (Ankle pain) : XM0Rs (Laterality) = 7NB32 (Left)

The full set of core terms, qualifiers and the linkages between them is
called a "post-coordination" schema. The set of core terms without
qualifiers or linkages is also known the "pre-coordinated set". These
features of pre- and post-coordination are also carried forward to
SNOMED-CT (although naming conventions change somewhat).

### 7.3.4 SNOMED CT

SNOMED CT came about in 2000 as the merger of CTV3 and SNOMED RT. The
latter began life with a pathology orientation (SNOP) in the 1960s but
grew over the decades to incorporate veterinary medicine and,
eventually, mainstream clinical medicine. In 2007 SNOMED CT became the
property of the IHTSDO, a not-for-profit organization currently
sponsored by its 9 original member countries and the 6 that have since
joined.

The technical characteristics of SNOMED are in many respects extremely
similar to CTV3: codes and terms have their own, separate identifiers;
concepts have a preferred term and multiple synonyms; individual terms
can be up to 255 characters in length (but there's no longer any notion
of different character length variants of the same term); single
concepts can appear in multiple places in the hierarchy; concept and
term codes can be moved and retired; there's a (more elaborate) system
of 'qualifiers' supporting post-coordination. Like CTV3 before it, many
of SNOMED's codes for complex clinical concepts are additionally
internally 'modeled' to be equivalent to bundles of more general codes.
Thus:

> 423827005\|Endoscopy (procedure)\|

...is also (within the system) known to be directly equivalent to the
bundle:

> 71388002\|Procedure\|:
>
> {260686004\|Method\|=129433002\|Inspection - action\|,
>
> 424226004\|Using device\|=37270008\|Endoscope\|}

Newer features of SNOMED include significantly more powerful ways of
defining and referencing arbitrary fragments of the content as (e.g. the
set of codes relating to a particular statutory or 'payment by result'
reporting activity, or the set of diseases of interest to a particular
outpatient clinic referable to via Choose and Book,), and additional
apparatus to support the international collaboration.

Because (almost) all of RV2s clinical content and terms were carried
through into CTV3 (minus, so far as possible, all pseudo-synonyms,
duplicates or ambiguous terms), and similarly all of CTV3s content is
carried through into SNOMED CT, anything that can be coded in RV2 can
also be coded in SNOMED using a single SNOMED code. The reverse,
however, is not true: SNOMED contains codes for many clinical concepts
that may be useful to GPs, but that can not be represented in RV2 at all
(or, though less commonly, in CTV3). It also contains many concepts
needed by specialities outside primary care.

### 7.4 General issues relating to terminology use

###

### 7.4.1 Concept or term selection

Unlike ICD, neither 4-Byte READ nor RV2 nor CTV3 were ever intended to
be published in a book format, as they are intended as a mechanism of
recording clinical information on computer. This 'computer orientation'
enables (and requires) different strategies and techniques for finding
the right code. You can't leaf through the codes in a book, and
something different to a 'back of the book' index is needed.

On typing in a term or string of characters, RV2 browser software
typically presents the user with lists of possible terms to choose,
where each displayed term is linked to a unique underling code which may
or may not also be visible. At no time is there an unavoidable need to
look up the codes themselves, or commit them to memory (though many
clinicians do), and in many systems the selected code itself is not
necessarily seen. Having chosen the term, the appropriate code is stored
in the background, while the term used is presented to the clinician in
the clinical record.

### 7.4.2 Variability of coding choices

It was originally intended that the need for detailed knowledge about
coding and classification by the clinician would be unnecessary: they
should be able to enter whatever free text phrase (or fragments of such
a phrase) come to mind at the keyboard, in the section of the record
where Read coding functionality is enabled, and without having to worry
much about the particular choice of words entered or the exact meaning
of the term or code actually selected from the search matches returned
by the system.

However, inspection of the coded records resulting from this approach
finds very wide variability -- both in what gets coded at all and in the
particular codes chosen for the same clinical phenomena but by different
clinicians (or by the same clinician on different days).

A significant cause of different clinicians selecting different codes is
*how* the list of possible codes to choose from is presented to the
clinician. Chiefly, this means in what order -- alphabetical, or more
commonly sorted according to some notion of which codes are selected
more frequently. Although such 'coding velocity' statistics might
theoretically be fixed and common across multiple practices, more
usually each installed system actively 'learns' what codes the
clinicians using it typically select, and constantly tunes the result
lists it presents accordingly. This strategy may speed local term
selection, but it can have the effect of perpetuating and to some extent
exaggerating the (mis) coding habits of individual practices or
clinicians and the idiosyncratic variability between practices.

There are also user interface differences between systems in how much of
the hierarchy around individual code/term choices is displayed by
default, and how easy it is to walk around the local term hierarchy from
a code that's nearly right to find one that's exactly right (or, to find
out for certain that a code you were *about* to choose because you
thought it was right actually means something entirely different).

The extent of variability in coding practices (different codes for the
same problem, or no code at all) is a significant problem for many of
the agencies tasked with extracting value from GP records. Despite the
not insignificant annual effort that clinicians are collectively putting
into coding their patient encounters, less clinical value can be
extracted from large collections of records than might be hoped or
expected. To improve on this situation, GPs, their staff and system
suppliers are already spending time on education and training to
understand and use the coding interface properly, rather than as a
natural language translation device. However, more training, more
sophisticated systems - and more sophisticated terminologies (SNOMED) -
will be required. Practice managers and data quality staff involved in
"data curation" for QOF and other 'data driven' NHS business processes
are perhaps most acutely aware of the problem.

### 7.4.3 Codes or Text?

The advantages of coded data entry, when used in the record, compared to
free text are as follows;

-   *Speed of data entry is quicker *

-   *Ambiguity of free text is diminished*

-   *Lexical confusion is diminished (cold (as in URTI) vs. Cold (feet),
    cold agglutinins etc.)*

-   *Once entered, data are significantly more readily searchable and
    retrievable than text, because of the inherent structure of the
    code*

-   *Information may be entered and retrieved (by running database
    queries or reports) in specific detail or in general detail because
    of the codes' hierarchical structure *

-   *Stored codes may be used by the record system for purposes of
    decision support*

In some circumstances there is no substitute for narrative text -- for
example when explaining details of the onset of depression, or as a
reminder of a patient's home circumstances. Narrative provides important
clinical context and detail that either can not be, need not be, or is
too time consuming to encode.

Remember that records, increasingly, may be shared. In general, it is
thought that free text entries are less safe to be shared because they
may contain sensitive information inadvertently. (See also "exclusion
subsets" below). Retrieval of free text information in database searches
is highly unreliable and slow.

**Figure 7.4.4 - Issues to remember with coded terminologies**

+-----------------------------------------------------------------------+
| There are many codes in the thesaurus. It is better to have agreement |
| with one's colleagues locally, and indeed wherever codes are shared,  |
| which codes should be used in a particular circumstance. For example  |
| in the case of asthma, consider whether it is truly important (or     |
| realistic to achieve accurately) to seek to record in code at such a  |
| granular detail as "intrinsic asthma" (or is "asthma" sufficiently    |
| expressive)?                                                          |
|                                                                       |
| If the collection, storage and retrieval of codes at an               |
| organisational level is extremely important, it may be wise to ensure |
| consistent coding by ensuring all clinicians use a template or        |
| protocol in specific circumstances -- for example when entering data  |
| important for long term condition recall, immunisations, QOF data,    |
| and so on. Be aware, however, that locally crafted templates provide  |
| another means to reinforce locally idiosyncratic coding choices.      |
| Unanticipated requirements to interoperate outside the original       |
| locale may be unusually complex or difficult to fulfil.               |
|                                                                       |
| Many systems allow free text to be associated with coded concepts.    |
| Never add free text which alters the meaning of the coded concept.    |
| For example;                                                          |
|                                                                       |
| **G30.. Acute myocardial infarction** (code) excluded (text)...       |
|                                                                       |
| would be strongly deprecated while the following is quite acceptable  |
|                                                                       |
| **G30.. Acute myocardial infarction** (code) developed chest pain at  |
| work (text)...                                                        |
|                                                                       |
| (See also Data Quality chapter 6.7.2)                                 |
+-----------------------------------------------------------------------+

### 7.4.5 Codes for other categories

All the examples given so far use diseases or diagnoses. However, Read
Codes and SNOMED also cover operative procedures, tests and test
results, prevention and administrative terms, drugs and much more.
Practices find them useful as tools with which to recall patients for
preventative screening and the management of long term disease, and they
are been helpful in the achievement of consistently high immunisation
rates in target populations throughout the UK.

### 7.4.6 Local codes

An important issue for all users of coded terminologies is the provision
of "local codes". These are codes, which are not universal in the coding
scheme, but are used in a limited number of practices, or only in a
single practice, or limited to a single system supplier. The standard
way of representing a local code in Read is in its chapter @\.... .
Systems suppliers may provide a user-base wide set of local codes (Egton
codes in EMIS is an example, or Y codes in TPP SystmOne[^6]).

Such codes may be useful for a local administrative purpose or if there
is an urgent need for a new code, which has not yet been incorporated
into the latest version of the codes centrally. E.g. if a new important
flu variant is diagnosed, it may take a few days for this to be
incorporated and so a local code might be added temporarily as a
placeholder, and when an appropriate national code is created the local
codes may be replaced.

**In general local codes should be avoided wherever possible, as they
will cause issues of interpretation when coded information is exported
from the practice, e.g. in GP2GP (qv), Summary Care Record, etc. Most
suppliers that enabled local code creation are now engaged in activities
to obtain official central codes to replace the commonly encountered
local codes found in live records. **

### 7.4.7 Search engines and RV2/CTV3 Termcodes

MIQUEST can only search on Read codes (Read 2 & CTV3) and is blind to
term codes / termIDs. MIQUEST searches can therefore only be set up on
the assumption that a given Read code will only represent the preferred
term. There are real world failing cases for this assumption (see e.g.
the N245. example earlier). It is a particular problem when a 'synonym'
term text is patently not a true synonym of the preferred term. The
classic example of this is where there is a term in RV2 "myocardial
rupture", a "so-called" synonym of myocardial infarction.

Some GP system searches are also similarly unable to run searches at the
termcode / termID level and so are similarly affected. This has
implications for audits and maybe also for DSS, and is also a challenge
for cross mapping, for example when moving from a system using RV2 to
CTV3 or SNOMED-CT. In these cases, the ideal map is not just concept to
concept, but concept and term to concept and description (the word used
in SNOMED-CT for a term).

### 7.4.8 Conceptid-termID binding

Principles underpinning clinical safety assurance of messaging demand
that the ConceptID termID and original term text should be preserved in
successive transfers to minimise risk of human and machine understanding
drifting apart.

### 7.4.9 The use of codes in the context of record structure.

In terminologies, concepts are given semantic tags, which define a
default "clinical context" for a concept, such as "disease" (as in
chapters A-T in RV2), symptom, procedure, and so on. But depending on
which GP system you are using, the information model of that system may
allow you to store and retrieve coded information in other than the
default context. In other words, if you wish to record a diagnosis of
"headache" (whilst evaluating the cause of a patient's headache), you
could record the *symptom code* for "headache" as a *placeholder* ,
until the diagnosis of the patients headache is clarified, then replace
"headache" with the disease code for "migraine". But beware, as some
systems cannot differentiate between symptoms used as diagnostic codes
from the default context of "symptom". In those systems, a code from
chapter "R" -- a \[D\] code -- can be used. (that is what they are there
for!)

### 7.4.10 Using codes and hierarchies to store and retrieve health data

As described above, the real power of hierarchical terminologies such as
Read, CTV3 and SNOMED-CT, lies in the ability to report on individuals
and groups of individuals who share characteristics which are coded on
the system. It is possible to identify all patients who are diagnosed
with a disease (for example Diabetes mellitus), and identify all of that
group that have been seen for a disease review (in this case diabetic
review) over a period of time (say the last 13 months). Or measure the
number of patients who have a given condition and who have had a
specific blood test measured in a given period; and what proportion have
had a result in the normal range (in our example what percentage of the
practice diabetic population has a recorded HBa1c of \<7.0mmol/l
recorded in the last 13 months.

The example used also illustrates the value of the coded terminology in
assessing performance and outcomes under the Quality and outcomes
framework (QoF).

Other examples might be tracing patients with a particular diagnosis who
are being treated with a particular drug - for example who are the
patients in the practice with a diagnosis of osteoarthritis who are
receiving regular medication with a non-steroidal anti-inflammatory drug
(NSAID)?

The hierarchy also allows searches for patients under a broad category
(e.g. Ischaemic heart disease) even when their conditions have been
coded much more specifically (e.g. inferior myocardial infarction).

### 7.5 Sharing coded information

###

As electronic communication of health information develops, new
considerations arise related to how we code information on our practice
computer systems. We can now transfer entire patient records from one
system to another when a patient changes practice (as in the GP2GP
record transfer), and post summary records to the Summary Care Record on
the "Spine" (SCR), or send messages which include free text and coded
information from point to point in electronic messages, and even secure
email. Another example is the automatically generated insurance report.

Such transfers of information are often partly automatic, and might
contain large amounts of information selected by code types. In general
it is wise to consider the following when sending coded information out
of the practice;

-   *Be very careful about any free text comments and notes exported. It
    is all too easy to miss a telephone number, and address or a
    reference to a third party and divulge sensitive personal
    information inadvertently*

-   *Consider whether ever to allow free text comments out of the
    practice in automatically generated reports*

-   *In some cases exclusion subsets will be applied to extracts from a
    coded record. It is wise to ensure at least one clinician or senior
    member of practice staff is conversant with Read codes and exclusion
    subsets to advise clinicians how to code and how to avoid disclosure
    of specific information inadvertently.*

-   *Always try to check what is being released under your authority as
    carefully as possible.*

### 7.5.1 Specific audits and reports written for export of practice data

In addition to the above there are mechanisms to write queries outside
the practice which can extract specific information about individuals or
groups of patients based on their characteristics coded in the record.
The most commonly used system is MIQUEST (Morbidity Information Query
Export Syntax). Built in to this system is a mechanism to anonymise the
patient (year of birth and first 3 characters of the postcode is the
maximum specifiable detail for an external query), and the ability for
the query to be scrutinised before being run, and the ability to see a
copy of the extract before it is released. Practices are advised to use
this functionality of MIQUEST to prevent inadvertent disclosure of
sensitive information to a 3^rd^ party. Never allow a query written by
someone you do not know and trust to be run on your practice system.

In the near future, we expect a new query system to be introduced,
currently being developed on behalf of the NHS Information Centre (NHS
IC) under the name of the GP extraction Service (GPES).

### 7.5.2 Codes and system to system messaging or system migration -- important guidance.

It is neither appropriate nor possible to try to discuss this important
issue in great detail here, as there are areas of surprising complexity
involved when migrating data from one coding scheme to another (see
Chapter 8c). Members of the informatics community of the RCGP and the
GPC have developed considerable expertise in this field, and advise the
NHS carefully about the rules and practical issues which must be
observed for safe migration of data. Try to be aware of the following
when your practice system is undergoing a migration to another system,
and also bear it in mind when you receive a GP2GP message from a system
with a dissimilar code scheme to your own.

1.  There are mapping tables for the following cases;

    a.  Read RV2 to CTV3

    b.  CTV3 to Read RV2

    c.  Read to SNOMED-CT

    d.  SNOMED-CT to Read

    e.  CTV3 to SNOMED-CT

    f.  SNOMED-CT to Read RV2

2.  For the above, a map at the code level is only acceptable if the
    term encoded for by the map target {code + termId} combination is
    identical to the original text of the term associated with the
    original coded concept and termId, OR if not identical then it has
    been clinically assured to carry the same meaning or a sufficiently
    similar meaning.

3.  If this is not the case, then the rules we endorse require the
    original text on the originating system to be carried to the target
    system, but no code in the target system is activated. This process
    is called "degrading to text", and a resulting entry in a GP2GP
    record transfer is referred to as a transfer degraded record entry
    (see Chapter 8b). It ensures that the actual text present on the
    original system is always seen in the new practice, but coded
    concepts with differences in meaning cannot be queried or reported

4.  In all cases we recommend that the originating code and text is
    stored and viewable on the target system

### 7.6 Preparing to move to SNOMED-CT, what to expect

The experience of the last 30 years has taught us that healthcare
computing is harder than it looks. Although the technologies and systems
developed in the 1980s and early 1990s still appear to function and
serve a useful purpose, they are creaking under the strain of modern
demands and expectations on data sharing and analysis. There is,
therefore, inherent long term risk in staying rooted in the past.

New technologies, including SNOMED CT, have been devised so far as
possible to fix the known failings of the older ones. There is some
near-term risk in adopting these more advanced solutions whilst they are
still to some extent in development but, conversely, unless they are
adopted they can not be tested and improved and so we shall remain stuck
in the past by default. SNOMED CT has emerged as the only serious
contender for an international standard 'next generation ' clinical
terminology; the resulting collaborative international working around
the emerging standard offers the prospect of faster, larger scale and
more robust testing and development than could happen were the UK to
continue building its own unique terminology products.

SNOMED CT is already deployed into live clinical systems in England,
including into the Choose and Book application, the NHS Summary Care
Record, hospice implementations of CrossCare, a tablet PC system for use
by paramedics first on scene, an A&E reporting system and all major
suppliers of new hospital systems including iSoft's Lorenzo and Cerner's
Millenium products. In primary care it forms the foundation of EMISWeb
while other supplier are actively developing next generation systems.

At the time of writing, therefore, it would seem likely that the major
GP suppliers are likely to produce and be seeking to deploy systems
supporting SNOMED-CT. Below is a brief account designed to offer a
flavour of the issues involved in the move to SNOMED-CT.

Past experience of migration from one coding scheme to another has
yielded useful lessons that inform us about the needed steps to achieve
successful migration. System suppliers are likely to rely heavily on
this experience in order to optimise the adoption of SNOMED. So we are
likely to see that the original text associated with a code in the
record will be retained, as well as the original concept code and term
code or description code. Not only will this help the user with the
provenance of the information, but will be invaluable if a record needs
to be transferred back to a different coding system in the future (if
for example a patient moves (GP2GP) or if a practice changes system.

In addition, GP suppliers will take great care to minimise the impact of
change from the user's perspective. One big issue with SNOMED-CT is the
size of the scheme (300 000 concepts, 1 million descriptions). As a
result of this there are at least 2 big issues for practices;

1.  Selecting a new code from the much bigger scheme without being lost
    in huge lists of specialist concepts, or not choosing the same
    concept each time for the same issue.

2.  Reporting using the hierarchical structure, which is different to
    both Read and CTV3 (significantly different from RV2, but more
    similar to CTV3)

In order to cope with this, GP system suppliers are likely to create a
"subset" or "refset" of SNOMED codes which is very similar to the set of
codes in their current system. They are likely to impose on this set of
codes a "navigational hierarchy" similar to the original scheme.

So if a practice moves from RV2 to SNOMED-CT, the read codes and term
codes would be preserved alongside the equivalent SNOMED-CT concept and
description codes. In addition, retrieval of data from the database
would be equivalent to the form of retrieval before the migration.
Issues would clearly arise as new concepts, which are in SNOMED-CT but
not the previous schema begin to be used, as then the retrieval queries
will have to be expressed in a way specific to SNOMED-CT concept
retrieval.

In essence this proposed implementation strategy will allow SNOMED-CT to
be used with minimal disruption to the clinician, but it also allows
system suppliers to control the pace of adoption of SNOMED-CT. Purists
may say that it will slow the pace of developing truly SNOMED-CT native
systems. Time will tell how effective this predicted strategy will pan
out.

A third and important "big issue" with SNOMED is in regard to
"post-coordination". Most (possibly all) of the concepts we currently
use in Read Version 2 and Clinical Terms version 3 will be carried
forward to SNOMED-CT because of the "superset principle". This implies
that initially at least, GP systems will be more or less fully
functional even without the need to cope with post coordination. However
many concepts, for example those used in many surgical procedures, do
not exist as single pre-coordinated concepts within SNOMED-CT. So,
concepts for laparascopic procedures are made up of several linked
concepts such as \<laparoscopic approach\> + \<appendicetomy\>. In
addition, for spine compliant systems, allergies are "conventionally"
represented (for the NHS) as \<substance allergy\> + \<substance\>;
similarly adverse drug reactions are represented as \<drug adverse
reaction\> + \<drug \[DM+D\] code\>. However the GP supplier wishes to
represent these things inside the system, they must be able to transform
the concepts into the "Proper" post coordinated expression when sending
information around the NHS.

Eventually we may expect that these systems will be able to cope with
the full expression of SNOMED in pre-coordinated forms, post coordinated
forms, and be able to compute equivalence of identical concepts
represented in different ways.

###

### Figure 7.7 - Glossary of words and phrases relevant to this chapter

  (Health) Classification     A categorisation of (health) concepts
  --------------------------- ------------------------------------------------------------------------------
  Code                        A label given to a (health) concept
  Coding                      The process of assigning codes to a record
  Concept                     The notion of an idea relating to a patient's health
  Conceptual Classification   An extensible set of concepts
  Description                 The word or phrase attached to a concept to describe its meaning in language
  Dictionary                  A list of words with their definitions
  Interface Terminology       A terminology designed for use in a particular application
  Lexicon                     A list of words used in a field of work without definitions

[^1]: Source: [The Health Improvement Network](http://www.thin-uk.com/)
    (THIN): 26,870,342 coded items added in 2006 to the records of
    2,596,459 patients registered to 339 practices in England (RCGP
    reported 10,352 practices in England in 2005; Population of England
    50,762,900 in 2006).

[^2]: JCG 20

[^3]: These are the \[D\] codes used to record uncertain diagnoses in
    symptomatic terms

[^4]: Actually, in practice, all synonym term codes used in the official
    RV2 data begin with a 1 or a 2. Higher term codes may be encountered
    'in the wild', but these are either instances of data corruption or
    originate from local, or supplier-wide (e.g. TermCode='99')
    extensions to the RV2 data.

[^5]: Practices in the network are asked to code each problem in the
    consultation with a diagnostic code, i.e. a code beginning with a
    capitalised letter. In cases where a diagnosis is uncertain, there
    is a series of \[D\] codes which enable symptoms to be
    differentiated from symptomatic diagnoses

[^6]: NB CTV3 proper include hundreds of thousands of codes beginning
    with Y or y; but they are (almost) all term codes not concept codes.
    Some cases of confusion have arisen because users have come across
    these and thought they were TPP (concept) local codes.
