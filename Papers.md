# What Papers Are Shown in News Compass?

News Compass focuses on **newsworthy tech research** that journalists and the public might care about. We focus on Computer Science papers for the time being, but a lot of the papers in the database are interdisciplinary research in practice.

## Papers We Include

**Sources:**
- **arXiv**: Latest preprints (CS + EESS categories)
- **OpenAlex**: Published CS articles  

**Category Filters**:
Across these sources, we require that papers speak to at least one of the following topic areas (`categories` in the arXiv API, and `subfields` in the OpenAlex API):

- AI / Machine Learning
- Computer Vision
- Natural Language Processing
- Robotics
- Human-Computer Interaction
- Computer Graphics
- Cryptography & Security
- Information Retrieval
- Social Networks
- Audio/Speech Processing, Image/Video Processing, Signal Processing

Realistically, this leads to a large amount of papers focused on core computer science, as well as those with an applied computer science bent (e.g., to biology, space, physics, social sciences, psychology).

**Quality filters**:
- Must have an abstract
- OpenAlex: published articles only (excludes editorials, book reviews)
- OpenAlex: specific subfields only (AI, Computer Vision, NLP, etc. - not theoretical CS)
- OpenAlex: Scopus-indexed journals only
