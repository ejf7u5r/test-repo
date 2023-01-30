## PR Checklist
### Common
- [ ] All the general, non-component-dependent constants used in a component are kept in nearest const file
- [ ] All the global constants used across many components are kept in global const file
- [ ] All the general, non-component-dependent functions used in a component are kept in nearest utils file
- [ ] All the global functions across many components are kept in global utils file
- [ ] There are no used consts, functions, components, imports, etc

### React
- [ ] Prop-drilling is avoided and replaced by store

### Performance
- [ ] Constants inside a re-rendering component are memoized using useMemo
- [ ] Callbacks / functions inside a re-rendering component are memoized using useCallback
- [ ] List / Grid / Table with large set of data is virualised / paginated as per applicable
- [ ] Nensted loops for large sets of data are avoided and if unavoidable, "find" on same array in loop is avoided by creating a MAP Object outside the loop and utlising same in loop.

### Unit test
- [ ] Unit test cases are added for all the changes made in this PR
- [ ] Skipped test cases (using xit()) have a TODO comment with justificaiton for skipping
