# patent-crsp-permco-match
These data provide a patent-CRSP permco match, as in our published paper, Stoffman, N., Woeppel, M., and Yavuz, M.D. 2022. Small Innovators: No Risk, No Return. Journal of Accounting and Economics. The data in our paper span 1976 through 2019. These data (patnum_permco_1976_2025.tsv) span 1976 through 2025.

If you use these data, please cite our paper as the data source.

| Variable | Description                               |
| -------- | ----------------------------------------- |
| patnum   | Patent number                             |
| fdate    | Filing date of patent (mm/dd/yyyy)        |
| idate    | Issue (grant) date of patent (mm/dd/yyyy) |
| permco   | CRSP permco                               |

These data span 1976 through 2025 and include only patents that we have matched the assignee to a firm in CRSP. In addition to string-matching algorithms, our extensive hand matching procedure helps resolves issues associated with mergers, acquisitions, asset sales, spin-offs, joint ventures, and other sources of inconsistency. For example, we match many patents assigned to two-party joint ventures to both owners of 50/50 joint venture. We plan to update these data at least annually.

Of the 8,057,116 utility patents with an assignee between 1976 and 2025, we match 3,098,245 or 38.5%, to CRSP firms. Our patent database includes 9,397 unique permcos matched to utility patents. 

We also include matches to non-utility patents that we did not use in our paper (patnum_permco_1976_2025_alt.tsv).

If you have any data issues or questions, please contact Mike Woeppel at mwoeppel@iu.edu.

*The quality of these data (i.e., accuracy of matches) benefited from the research assistance of Garrett Klinge.

