# UnitTest

## 3 way to write clear unit test
- [Unit Test Guide](https://blog.usejournal.com/3-easy-ways-to-write-cleaner-unit-tests-2ec04ca6b9df)

### 1. One test, one function
### 2. Good test names

Structure test names in the following way: 

```
  public void testSYSTEM_BEHAVIOR_CONDITION(){
  ...
  }

```

For example: 
```
  public void testAuthenticate_rejectsUser_whenBadCredentialsProvided(){
  ...
  }
```

### 3. AAA: Arrange, Act, Assert 

  - Arrange : 
             setup the test.
             Mock outgoing RPCs, populate fake databases, etc.
  - Act     :
             Run the function under test.
  - Assert   :
             Check that the expected behavior occurred.

```
   public void testMyFunc_updateBar() {
       Bar bar;
       Bar expectedBar = makeBar().setBuzzer(3);
       myFunc(bar);
       assertThat(bar).isEqualTo(expectedBar);
}

```


  
 

