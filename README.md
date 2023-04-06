# ng-azure-pipeline
An Angular multi-stage azure build and deploy pipeline targeting multiple environments.

stages
- [x] install dependencies or use cache (pr & merge)
- [ ] test (pr & merge)
- [ ] build (pr & merge)
- [ ] deploy (merge)
  - [ ] dev (merge to develop branch only)
  - [ ] qas (merge to release/* branch only)
  - [ ] prd (merge to main branch only)

triggers
- pr from fix/* or feature/* into develop
- pr from fix/* into release/*
- pr from release/* into main
- merge into develop
- merge into release/*
- merge into main