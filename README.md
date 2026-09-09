# Cybersecurity research artifacts extracted by ArtiFinder

This repository contains automatically extracted artifact links from cybersecurity papers.
The dataset currently contains all papers published between 2000--2025 at IEEE S&P, ACM CCS, NDSS, and USENIX Security, and all papers published between 2017--2025 at ACSAC.
To manually validate entries or submit corrections, please submit a pull request or an [issue](https://github.com/DistriNet/ArtiFinder-Data/issues/new?template=validation.yml).

For more information, please refer to the [ArtiFinder](https://github.com/DistriNet/ArtiFinder) repository and our USENIX Security 2026 [paper](https://daanvs.be/files/usenix-share.pdf):

```bibtex
@inproceedings{vansteenhuyse26notall,
  title     = {Not All Those Who Share Are Lost: Analyzing 25 Years of Cybersecurity Artifact Sharing Practices Through Automated Discovery},
  author    = {Vansteenhuyse, Daan and Bols, Arthur and Desmet, Lieven and Le Pochat, Victor and Van Bulck, Jo and Bognar, Marton},
  year      = 2026,
  booktitle = {USENIX Security},
}
```

The repository contains records on all papers in the following format:

```yaml
  # title of the paper
- title: 'Libra: Architectural Support For Principled, Secure And Efficient Balanced Execution On High-End Processors.'
  # list of authors
  authors:
  - Hans Winderix
  - Marton Bognar
  - Lesly-Ann Daniel
  - Frank Piessens
  # link to the published paper
  page_link: https://doi.org/10.1145/3658644.3690319
  # a list of all links discovered by ArtiFinder above our score threshold, ordered from highest to lowest score
  # an empty list indicates no artifact link found
  artifacts_discovered:
  - https://github.com/proteus-core/libra
  - https://doi.org/10.5281/zenodo.12786159
  # flag indicating that the entry has been manually validated (and possibly corrected)
  validated: true
  # flag indicating that the artifact URL is not present in the published paper (was manually added to the database)
  not_present: true
```

## Note on the order of authors in records

We have noticed that the author order on certain NDSS papers is incorrect on both the conference website and DBLP, and as a result, also in our database.
Fixes to these records (just as all other corrections) are very welcome in a pull request.
