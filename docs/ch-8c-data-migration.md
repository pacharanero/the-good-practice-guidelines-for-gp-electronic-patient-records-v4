---
title: 8c. Data Migration
---

# 8c. Data Migration

### **8c.1 Formalising the process of data migration**

The Data Migration Improvement Project (DMIP) was set up to improve the
quality of data migrations between source and target systems using
different software, typically provided by different suppliers. Under GP
Systems of Choice (GPSoC) arrangements, individual suppliers' data
migration processes are assessed against a set of requirements developed
by DMIP. These requirements are predicated on a clearly defined end to
end process and careful planning. They effectively set a standard for
all data migrations between GP systems. The aim is to minimise
disruption to practices and to keep the loss / modification of
information resulting from the data migration process to a minimum
thereby reducing risks to patient safety.

### **8c.2 Data migration process**

A well-organised data migration process should progress through the
following stages;

1.  Preparation and planning

2.  Extraction of data from source system

3.  Transformation / translation of data from source system format to
    target system format

4.  Import of transformed / translated data to target system

5.  Handling of exceptions and review of data in target system

6.  Iteration as necessary of steps 2 -- 5 until a satisfactory result
    is obtained at step 5

7.  'Cut over' to target system

8.  Back-loading to target system of any data collected during the
    period of time from the final source system data extraction to
    target system 'cut over'

9.  Review of information in target system in 'live'

10. Final sign off

These stages are considered in more detail below.

### **8c.2.1 Preparation and planning**

This is the most important stage as the smooth running of the whole
process is dependent upon careful planning. The preparation and planning
should start from the point at which a decision is being made as to
whether or not the practice system should be changed (i.e. the decision
upon which the need to undergo data migration depends). In particular it
should take full account of the possible disruption to established
practice routines that may result. A typical modern general practice
will have modified its business processes over the years to the extent
that almost every aspect of its work will now be more or less dependent
on its computer system. It has been suggested that the overall
efficiency of a practice will typically drop at the time of migration
and then take up to six months to recover to its original level. Reasons
for this include the need for;

-   *Members of the practice team to become familiar with the workings
    of a new system*

-   *Some tasks to be carried out differently*

It is therefore important to identify which aspects of the practice's
work are likely to be most affected, for example in the reception area,
consultation room or back office, and then to work out effective ways of
making the necessary transition. Particular consideration should be
given to the training needs of both clinical and non clinical staff.

The actual process of data migration will itself make demands on
practice resources. Practices should consider nominating a lead person
to work with the target system supplier who would start with the
planning process and then go on to manage and coordinate the involvement
of practice resources at successive stages. The supplier should be able
to provide a template outlining all of the processes in sequence, the
points at which practice input will be required and the nature of that
input. The plan should include clear milestones, define roles and
responsibilities and identify how communications will be managed. In
particular it should cover;

-   *Unambiguous definition of what information must be migrated*

-   *Clear identification of what information will not be migrated*

-   *Discussion of known incompatibilities between source and target
    systems and how these should be handled*

-   *Business continuity arrangements. Depending on the process followed
    by the supplier one backup is likely to be identified as 'final'.
    Details about filing of pathology results, letters etc before this
    final backup should be agreed with the supplier. There may be a
    period between the time of this final backup and the time of 'cut
    over' to the new system when any entries made on the source system
    will never be migrated to the new system. Some suppliers are able to
    take an incremental backup which sweeps up all such entries and
    migrates them to the new system but others do not do this. It is
    important to discuss this in detail with the supplier and to
    determine the likely duration of any such period. There may be a
    need to maintain an alternative recording system (e.g. on paper) of
    all key transactions during this period so that these can eventually
    be 'back-loaded' into the new system after 'cut over'. It so, the
    arrangements should be carefully planned and communicated to the
    whole practice. This time gap should be kept as short as possible
    (i.e. days)*

-   *Clarity about the practice's current system back-up routine
    including any encryption measures: there will be a need for full
    backups to be provided at specific times as the data for migration
    is usually extracted from back-up tapes*

-   *Clear policy on the handling of updates (e.g. of Read codes / drug
    codes / source system patches etc.) during the data migration
    process*

-   *Maintenance of any existing interfaces with other Practice IT
    systems / equipment*

-   *Conformity with current clinical safety approach (at the time of
    writing the Connecting for Health Clinical Safety Approach)*

-   *Compliance with Information Governance best practice*

-   *Cataloguing and explanation of tools etc. to be used (e.g. cross
    maps / means of finding irregularities in source data, determining
    the quality of information migrated to target system)*

-   *Maintenance of access to the original source system during and
    after the migration process so that where necessary patient records
    can continue to be accessed. This is likely to require liaison with
    the PCO*

### **8c.2.2 Extraction of data from source system**

The supplier may at different times wish to request a full backup of
practice data. These should be planned to occur at times that cause
minimum disruption to practice business.

### **8c.2.3 Transformation / translation of data from source system format to target system format**

Carried out by the target system supplier (or by a third party on that
supplier's behalf) usually away from the Practice

### **8c.2.4 Import of transformed / translated data to target system**

In the early stages this may be done away from the Practice. The new
target system should be set up at an early stage in the data migration
process with a 'dummy' database available for training and
familiarisation. This should be separate from any database into which
live data may be imported

### **8c.2.5 Handling of exceptions and review of data in target system**

The supplier may be able to offer a choice as to what should be done
with parts of the data that cannot be automatically transformed /
translated from the source system format to the target system format.
This may result from differing structures, differing coding systems /
use of System or Practice local codes etc. There should be close
collaboration between supplier and trusted member(s) of the Practice.
See below for iterative nature of this process and the importance of
reviewing the quality of the data migration.

### **8c.2.6 Iteration as necessary of steps 2 -- 5 until a satisfactory result is obtained**

The majority of this work will not involve the practice. In general most
of the transformation / translation will be automatically carried out by
the supplier (or by a third party on the supplier's behalf) through the
use of a piece of pre-existing software known as an 'adaptor'. However,
there will be a need for some practice input at various points (e.g.
where the supplier can offer a choice as to what should be done with
parts of the data that cannot be automatically transformed / translated
to the target system). It is important that this input should be
forthcoming from a trusted member of the practice with (delegated)
authority who may wish to involve other members of the practice when
appropriate. The practice should not allow the final 'cut over' to take
place until satisfied with the quality of the data migration.

### **8c.2.7 'Cut Over' to target system**

It should be noted that at this point the target system becomes the
primary record system for the practice (i.e. used in place of the
original source system).

### **8c.2.8 Back-loading to target system of any data collected during the period from time of final data extraction from source system to time of 'cut over' to target system**

See above 'Business continuity' under 'Preparation and planning'

### **8c.2.9 Review of information in target system in 'live'**

Practices should participate actively in reviewing the migrated
information in the 'live' environment. Typically suppliers will have
procedures / tools that can demonstrate that all patient records on the
source system have been migrated and that simple searches (e.g. for QOF
points, diagnoses etc.) yield comparative numbers. These should have
been covered during preparation and planning.

### **8c.2.10 Final sign off**

At the time of writing, under GPSoC rules, the data migration must be
signed off both by the practice and by the PCO. Practices should ensure
that they have thoroughly reviewed the information in the new system and
are satisfied with the results. Practices **must** undertake a
comparison of records between the old and new systems as they retain
ultimate responsibility under the Data Protection Act for ensuring that
the data has been migrated correctly (see Chapter 4.2.4).
