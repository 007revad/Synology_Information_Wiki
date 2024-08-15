From [Synology's Software_Life_Cycle_Policy_enu.pdf](https://global.download.synology.com/download/Document/Software/WhitePaper/Os/DSM/All/enu/Software_Life_Cycle_Policy_enu.pdf) - 
Last updated: Jul 2, 2024


### DiskStation Manager (DSM)

DSM follows the MAJOR.MINOR.MICRO-BUILD-NANO versioning rules:

- MAJOR version is for incompatible system behavior or API changes
- MINOR version is for new functionality in a backward-compatible manner
- MICRO version is for incremental security or bug fix updates
- BUILD is an additional engineering identification of the release
- NANO version is for a specific security or bug fixes with backward compatibility

Each minor version of DSM, such as DSM 6.2, is identified as a different product with a different
number of life-cycle phases. Some of them will have an extended life phase and are identified as
long-term support. Security fixes, bug fixes, software enhancements, or hardware enablements
may be contained in each phase.

Software changes to DSM will be delivered via individual nano updates as minimum changes, such
as DSM 6.2.2-24922-4, or be aggregated as an incremental release, such as DSM 6.2-23739 or
6.2.2-24922.

The following table lists the differences between each release version:

|  | Major Release | Minor Release | Micro Release | Nano Release |
|--|--|--|--|--|
| Examples (Naming) | DSM 6.0-7321 | DSM 6.2-23739 | DSM 6.2.2-24922 | DSM 6.2.2-24922-4 |
| Release: Frequency | Years | Years | Quarters | Months |
| Release: Basis | Schedule | Schedule | Schedule | Incident |
| Includes: Features | Yes | Yes¹ | Yes¹ | No |
| Includes: Criteria | Liberal | Strict¹ | Strict¹ | Very Strict |
| System ABI Guaranteed | No | No | Yes | Yes |

1. Depends on the life-cycle phase.
