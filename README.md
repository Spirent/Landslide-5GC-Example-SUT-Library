# Landslide-5GC-Example-SUT-Library
The Landslide 5GC Automation Package Example SUT Library repository contains stubbed SUT function calls to serve as an example or starting point used when testing a real SUT. 

When running Landslide 5GC automated tests run back-to-back, functions in the SUT library are not called. However, the Landslide 5GC project is **dependent** upon this one, so it must be defined as one of the remote repositories in the Landslide 5GC Velocity repo. This remote repository along with the [Landslide 5GC repository](https://github.com/Spirent/Landslide-5GC.git) needs to be defined in your Velocity SCM in order for the Landslide 5GC test cases to operate properly, for example:

![Repo](ai_SUT_Library/documentation/velocity.repo.1.png)

When testing a real SUT with the Landslide 5GC automated test suite, functions in this libary are called to fetch KPIs like CPU and memory consumption. These functions can also be enriched to perform any SUT assertion, to set customized pass/fail verdicts, or to fetch other interesting KPIs that should be recorded in the test report and, optionally, in Elasticsearch for trend analysis.


