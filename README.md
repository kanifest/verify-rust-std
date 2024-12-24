# Rust std-lib verification

To run the verification harnesses we defined for `std::string::String`, go into the root of the project and run:

```
# Run all, could take hours
./scripts/run-kani.sh --kani-args "--harness string::verify::check_"
# Run just one, for example, check_remove_one (takes least time, ~20 minutes including building the std library)
./scripts/run-kani.sh --kani-args "--harness string::verify::check_remove_one"
```