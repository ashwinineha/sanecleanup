# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [2.0.0] - 2021-03-23

### Changed

- Cleanup jobs / retention rules are now imported on-demand based on the extensions the project uses.

### Added

- Custom retention cronjob to replace CMS Version [Garbage Collection][versiongc].\
  The ootb garbage collection mechanism is over-engineered and should be a regular cronjob.
  
- Retention rules and jobs for the promotion engine, based on [Top 10 Recommendations for Improving the Performance of your Commerce Cloud Promotion Engine][top10]

[versiongc]: https://help.sap.com/viewer/9d346683b0084da2938be8a285c0c27a/2011/en-US/9089116335ac4f4d8708e0c5516531e3.html
[top10]: https://www.sap.com/cxworks/article/538808299/top_10_recommendations_for_improving_the_performance_of_your_commerce_cloud_promotion_engine

## [1.0.1] - 22020-12-09

### Added

- Bulk cleanup cronjob for log files - useful for a one-time cleanup before the retention 
  job for job logs is enabled

## [1.0.0] - 2020-11-26

Initial release

### Added

- Cleanup for:

    - CronJobs
    - CronJob Histories
    - Lob Logs / Log Files
    - Impex Media
    - HTTP Sessions
    - Business Processes
    - Carts

[Unreleased]: https://github.com/sap-commerce-tools/sanecleanup/compare/v2.0.0...HEAD
[2.0.0]: https://github.com/sap-commerce-tools/sanecleanup/compare/v1.0.1...v2.0.0
[1.0.1]: https://github.com/sap-commerce-tools/sanecleanup/compare/v1.0.0...v1.0.1
[1.0.0]: https://github.com/sap-commerce-tools/sanecleanup/releases/tag/v1.0.0
