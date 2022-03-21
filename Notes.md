1. #### Which function will be part of the ABI?
```
contract A {
  string public str;

  function foo() external {
      str = "foo";
  }
  function bar() public {
      str = "bar";
  }
  function baz() internal {
      str = "baz";
  }
  function bax() private {
    str = "bax";
  }
}
```
**Answer**: Only "foo" and "bar", "baz" is internal function only visible in this contract and derived contracts. "bax" is only visible inside this contract
