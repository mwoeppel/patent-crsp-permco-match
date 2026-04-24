# patent-crsp-permco-match
These data provide a patent–CRSP permco match, as in our published paper: Stoffman, N., Woeppel, M., and Yavuz, M.D. (2022), Small Innovators: No Risk, No Return, Journal of Accounting and Economics. The data used in the paper span 1976 through 2019. The dataset here (patnum_permco_1976_2025.tsv) covers 1976 through 2025 and is based on a full rematching of the data.

If you use these data, please cite our paper as the data source.

| Variable | Description                               |
| -------- | ----------------------------------------- |
| patnum   | Patent number                             |
| fdate    | Filing date of patent (mm/dd/yyyy)        |
| idate    | Issue (grant) date of patent (mm/dd/yyyy) |
| permco   | CRSP permco                               |

This dataset covers U.S. patents from 1976 through 2025 and includes only patents where we were able to match the assignee to a firm in CRSP.

We use a mix of string-matching algorithms and a lot of manual checking to link patents to firms. The manual work helps deal with things like mergers, acquisitions, asset sales, spin-offs, joint ventures, and other inconsistencies in firm names. For example, when a patent is assigned to a two-party joint venture, we match it to both firms if it’s a 50/50 split.

This is the first time since building the dataset in 2020 that I updated the matching algorithm. The new version is designed to reduce both false matches (Type I errors) and missed matches (Type II errors). I also spent significant time improving the manual matching, adding hundreds of lines of code.

Out of 8,057,116 utility patents with an assignee between 1976 and 2025, we match 3,098,245 of them (38.5%) to CRSP firms. In total, the dataset includes 9,397 unique permcos.

We also include matches to non-utility patents, which were not used in our paper. These are in the file patnum_permco_1976_2025_alt.tsv.

If you have any data issues or questions, please contact Mike Woeppel at mwoeppel@iu.edu.

*The quality of these data (i.e., accuracy of matches) benefited from the research assistance of Garrett Klinge.
