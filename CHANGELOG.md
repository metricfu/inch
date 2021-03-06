# Changelog

## 0.3.3

- Fix rake task
- Remove unused constant
- Add support for overload tag
- Add failing test re: method overloading
- Update README with configuration instructions


## 0.3.2

- Fix bug when parsing .inch.yml
- Separate test suite in unit and integration tests
- Support regexes in .inch.yml
- Add some basic ideas for .inch.yml support
- Speed up tests by caching code objects


## 0.3.1

- Fix error with empty docstring
- Do not count @raise tag if it is auto-assigned via YARD
- Add a role to encapsulate notations of private tags
- Update Docstring to detect internal apis
- Fix output of priority arrows in Suggest command
- Use original docstring to determine if an object is undocumented?
- Fix things complained about in last commit
- Exclude failing test
- Don't apply transitive :since tag to children's evaluation
- Fix bug in YARD method object proxy
- Fix wrong detection of splat and block parameters
- Fix 1.9.3 compatibility of Inch::Utils::UI
- Fix #depth method
- Add Inch::Utils::UI utility class
- Cache some repeatedly calculated values


## 0.3.0

- Add proxy for RootObject to YARD object provider
- Ignore some YARD code objects by type
- Remove YARD from core_ext
- Fix bug showing wrong paths instead of files in Suggest
- Ensure output if Suggest has nothing to suggest
- Merge pull request #5 from splattael/perf
- Upgrade to Ruby 2.1 as default
- Prefer `Module#const_get(class_name)` over `eval(class_name)`
- Prefer `public_send(name)` over `method(name).call`
- Perf: Index codeobjects objects by fullname
- Merge pull request #4 from jimjeffers/master
- Fixed minor typo in CLI for suggest command.
- Require 'forwardable' at the very top
- Add fix for failing test
- Add failing test fixture
- Refactor Evaluation namespace
- Add doc to ObjectsFilter
- Add CodeObject::Provider modules
- Rewrite Evaluation Role model
- Add some more docs
- Extract shared specs into own file
- Depend on minitest ~> 5.2
- Merge pull request #3 from splattael/simplecov
- Add docs to ReadWriteMethods
- Move simplecov's configuration into own file
- Add tests for new API classes
- Rename Evaluation::WeightedList -> Utils::WeightedList
- Fix description of stats command
- Add PriorityRange
- Refactor inspect/show output
- Introduce API namespace
- Fix wrong command registration in Command::Inspect
- Add Codebase::ObjectsFilter
- Update commands to use Codebase
- Introduce Codebase namespace
- Remove unused method alias
- Fix bug in Docstring


## 0.2.3

- Bump version
- Rescue error raised by YARD
- Let Command classes register themselves in CommandParser
- Fix failing tests (typo)
- Refactor some more methods
- Refactor complex methods
- Add Getter and Setter roles
- Refactor ScoreRanges into GradeLists
- Add Inch::Config
- Rename Evaluation::Criteria -> ObjectSchema
- Add weighted_list for suggest output
- Make CodeObject::Proxy#object an attr_reader


## 0.2.2

- Fix bug related to private @api tags (again)


## 0.2.1

- Fix bug related to private @api tags


## 0.2.0

- First public release
