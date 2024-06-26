# DPVCG
Data Privacy Vocabularies and Controls Community Group (DPVCG) repository

[Community Group](https://www.w3.org/community/dpvcg/) | [(W3C) wiki](https://www.w3.org/community/dpvcg/wiki/Main_Page)
  
> **MAJOR CHANGES introduced in v2**
>
> The scope of DPV has been expanded to include non-personal data and AI technologies - though the focus of the group remains on privacy and data protection. The structure of the repo has also been changed to incorporate multiple jurisdictions and regulations, and their names have been changed e.g. `dpv-gdpr` is `legal/eu/gdpr`. Versioned IRIs have been created to refer to specific versions, with https://w3id.org/dpv/1.0 for v1 and https://w3id.org/dpv/2.0 for v2. The versionless IRI https://w3id.org/dpv will always point to the latest version. Read more in [v2 changelog](https://w3id.org/dpv/2.0/changelog). 

> The draft article [Data Privacy Vocabulary (DPV) -- Version 2](https://arxiv.org/abs/2404.13426) by Pandit et al. (2024) describes DPV v2 in terms of its contents, methodology, current adoptions and uses, and future potential. It also describes the relevance and role of DPV in acting as a common vocabulary to support various regulatory (e.g. EU's DGA and AI Act) and community initiatives (e.g. Solid) emerging across the globe

The mission of the W3C Data Privacy Vocabularies and Controls CG (DPVCG) is to develop a taxonomy of privacy and data protection related terms, which include in particular terms from the new European General Data Protection Regulation (GDPR), such as a taxonomy of personal data as well as a classification of purposes (i.e., purposes for data collection), and events of disclosures, consent, and processing such personal data.

> Newcomers to the DPV are recommended to start with the [Primer](https://w3id.org/dpv/primer) to familiarise themselves with the concepts, semantics, and usefulness of the DPV.

License: All work produced by DPVCG and provided through this repo or elsewhere is provided by contributors under the [W3C Document License](https://www.w3.org/copyright/software-license-2023/). A copy of the license is provided in the [LICENSE.md](./LICENSE.md) file.

[Guidelines for contributing](https://github.com/w3c/dpv/wiki/contributing)

## Specifications
### Data Privacy Vocabulary (DPV)
The [Data Privacy Vocabulary (DPV)](https://w3id.org/dpv) provides an ontology (classes and properties) and taxonomies of concepts to represent information regarding how personal data is processed in the form of an ontology or a knowledge graph. For example, it provides taxonomies associated with:

* purposes of processing
* personal data categories involved
* processing operations
* technical and organisational measures or restrictions applied
* legal basis used to justify processing
* information about legal basis for processing
* rights as applicable
* risks as applicable

The namespace for DPV terms is `http://w3id.org/dpv#` with suggested prefix `dpv`, and serialisations are provided in RDF/XML, Turtle, JSON-LD, and N3 formats. The default serialisations are defined using RDFS/SKOS semantics, with an [alternate serialisation](https://w3id.org/dpv/dpv-owl) defined using OWL2 semantics.

### Extensions
These extensions provide additional concepts that extend the concepts and scope of the main DPV specification:
- [Personal Data (PD)](https://w3id.org/dpv/pd) provides a taxonomy of personal data categories
- [Location (LOC)](https://w3id.org/dpv/loc) provides a taxonomy of location concepts based on ISO 3166 (countries, regions)
- [Technology (TECH)](https://w3id.org/dpv/tech) provides a taxonomy of technology concepts
- [AI](https://w3id.org/dpv/ai) provides a taxonomy of AI concepts extending the TECH extension
- [Justifications](https://w3id.org/dpv/justifications) provides concepts for representing justifications i.e. why something must be done or could not be done
- [Risk](https://w3id.org/dpv/risk) provides concepts for risk assessment and management

### Extensions for Jurisdictions and Regulations
The legal extensions provide concepts associated with specific jurisdictions and the laws, authorities, and treaties within them. The [Legal](https://w3id.org/dpv/legal) page provides an overview of these. The jurisdictions are represented by using their ISO 3166-2 codes.

- [European Union (EU)](https://w3id.org/dpv/legal/eu)
    - [GDPR](https://w3id.org/dpv/legal/eu/gdpr)
    - [DGA](https://w3id.org/dpv/legal/eu/dga)
    - [AI Act](https://w3id.org/dpv/legal/eu/aiact)
    - [Charter of Fundamental Rights](https://w3id.org/dpv/legal/eu/rights)
- [Germany (DE)](https://w3id.org/dpv/legal/de)
- [Ireland (IE)](https://w3id.org/dpv/legal/ie)
- [India (IN)](https://w3id.org/dpv/legal/in)
- [United Kingdom (GB)](https://w3id.org/dpv/legal/gb)
- [United States of America (USA)](https://w3id.org/dpv/legal/usa)

### Other Resources
The [NACE Taxonomy serialised in RDFS](https://w3id.org/dpv/dpv-nace) provides a serialisation of the NACE v2 taxonomy in RDFS for use with DPV terms. Since then, NACE v3 has been published with an updated taxonomy. The DPVCG is looking into whether the NACE v3 should be similarly provided.


## Guides
- The [Primer](https://w3id.org/dpv/primer) is an introductory document for newcomers to understand the DPV and its concepts. A [2 Page Short Primer](https://w3id.org/dpv/primer/short) provides a succint introduction to the DPV. 
- The [Use-Cases and Requirements](https://w3id.org/dpv/use-cases/) document lists the use-cases and requirements that led to the development of DPV. 
- The [Examples](https://w3id.org/dpv/examples/) page provides an index of examples describing the use of DPV concepts.
- The [Guides](https://w3id.org/dpv/guides) page lists guides for use of DPV in specific domains and applications
    - [Using DPV in OWL2](https://w3id.org/dpv/guides/dpv-owl) 
    - [Implementing ISO/IEC 27560:2023 Consent Records and Receipts](https://w3id.org/dpv/guides/consent-27560)
    - [Implementing ISO/IEC 29184:2020 Privacy Notices and Consent](https://w3id.org/dpv/guides/notice-29184) - Work in Progress
    - [Data Breach Management for GDPR](https://w3id.org/dpv/guides/gdpr-data-breach) - Work in Progress
    - [Data Protection Impact Assessment (DPIA) for GDPR](https://w3id.org/dpv/guides/gdpr-dpia) - Work in Progress
    - [Records of Processing Activities (ROPA) for GDPR](https://w3id.org/dpv/guides/gdpr-ropa) - Work in Progress

## Acknowledgements and Citation

*  For use of DPV up to v1 and v1.1, **Cite as:** The peer-reviewed article “[Creating A Vocabulary for Data Privacy](https://link.springer.com/chapter/10.1007%2F978-3-030-33246-4_44)” presents a historical overview of the DPVCG, and describes the methodology and structure of the DPV along with describing its creation. An open-access version can be accessed [here](http://hdl.handle.net/2262/91581), [here](http://doras.dcu.ie/23801/), and [here](https://aic.ai.wu.ac.at/~polleres/publications/pand-etal-2019ODBASE.pdf).
* For use of DPV from v2 onwards, **Cite as:** [Data Privacy Vocabulary (DPV) -- Version 2](https://arxiv.org/abs/2404.13426) by Harshvardhan J. Pandit, Beatriz Esteves, Georg P. Krog, Paul Ryan, Delaram Golpayegani, Julian Flake https://arxiv.org/abs/2404.13426 (2024)

## Releases

> [go to latest release](https://github.com/w3c/dpv/releases/latest)

Releases are provided through the GitHub feature at [https://github.com/w3c/dpv/releases](https://github.com/w3c/dpv/releases) and contain zipped collections of DPV specifications, modules, extensions, and accompanying documents, categorised by serialisation. 

- dpv (`dpv.zip`) : canocical specifications serialised in RDFS/SKOS
- dpv-owl (`dpv-owl.zip`) : alternate serialisation with OWL2 semantics
- dpv (`dpv.xlsx`) : DPV's terms provided in a spreadsheet

### Final Reports

The following are final reports i.e. formally published by the W3C:
#### v2
- these reports will be published and available after the release of v2
#### v1
- Primer [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-primer-20221205)
- DPV [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-20221205)
- DPV-GDPR [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-gdpr-20221205)
- DPV-PD [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-pd-20221205)
- DPV-OWL [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-owl-20221205)
- DPV-OWL-GDPR [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-owl-gdpr-20221205)
- DPV-OWL-PD [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-owl-pd-20221205)
- Guide on using DPV in OWL2 [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-guide-dpv-owl-20221006)
- DPV-SKOS [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-skos-20221205)
- DPV-SKOS-GDPR [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-skos-gdpr-20221205)
- DPV-SKOS-PD [w3c/cg-reports link](https://www.w3.org/community/reports/dpvcg/CG-FINAL-dpv-skos-pd-20221205)

## Participating and Getting assistance

If you're unsure about something, or would like clarifications, or suggestions - please communicate with us or open an issue. We would be happy to help. You can view the [current open issues](https://github.com/w3c/dpv/issues) and the [public mailing list](https://lists.w3.org/Archives/Public/public-dpvcg/).

Membership to the group is open to all interested individuals and organisations. To join the group, you need a valid W3C account – which is free to get and can be [requested here](https://www.w3.org/accounts/request). The group meets usually through online meeting calls - see [meetings calendar](https://www.w3.org/groups/cg/dpvcg/calendar) and [minutes](https://w3id.org/dpv/meetings/).

