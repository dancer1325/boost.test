![boosttest logo](doc/html/images/boost.test.logo.png)

# What is Boost.Test?
* == C++11/14/17 unit testing library
  * ALLOWED |
    * platforms
    * compilers
  * part of [Boost](http://www.boost.org)

# Key features

* TODO:powerful and unique test assertion macro [`BOOST_TEST`](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/testing_tools/boost_test_universal_macro.html), that understands floating points, collections, strings... and uses appropriate comparison paradigm
* self-registering test cases, organize cases in test suites, apply fixtures on test cases, suites or globally
* provide assertion [context](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/test_output/test_tools_support_for_logging/contexts.html) for advanced diagnostic on failure
* powerful and extensible [dataset](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/tests_organization/test_cases/test_case_generation.html) tests
* add [decoration](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/tests_organization/decorators.html) to test cases and suites for [advanced description](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/tests_organization/semantic.html), [group/label](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/tests_organization/tests_grouping.html), and [dependencies](http://www.boost.org/doc/libs/release/libs/test/doc/html/boost_test/tests_organization/tests_dependencies.html)
* powerful command line options and test case filters
* extensible logging, XML and JUNIT outputs for third-party tools (eg. cont. integration)
* various usage (shared/static library/header only) for faster integration and/or compilation/build cycles, smaller binaries

# how to get started?
* TODO: 
1. download and deflate the latest boost archive
1. create a test module with this (header version):
    ```
    #define BOOST_TEST_MODULE your_test_module
    #include <boost/test/included/unit_test.hpp>
    ```
1. Write your first test case:
    ```
    BOOST_AUTO_TEST_CASE( your_test_case ) {
        std::vector<int> a{1, 2};
        std::vector<int> b{1, 2};
        BOOST_TEST( a == b );
    }
    ```
1. build and run
1. done

# documentation
* [here](doc/test.md)
