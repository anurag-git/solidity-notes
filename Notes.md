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
