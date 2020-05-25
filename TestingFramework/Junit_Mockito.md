# JUnit
Step 01 : Need for Unit Testing
Step 02 : Setting up your First JUnit 
          --Add Dependency in build path.
Step 03 : First Successful JUnit. Green Bar and assertEquals
Step 04 : Refactoring Your First JUnit Test
Step 05 : Second JUnit Example assertTrue and assertFalse
Step 06 : @Before @After
Step 07 : @BeforeClass @AfterClass
Step 08 : Comparing Arrays in JUnit Tests
        By assertArrayEquals().
Step 09 : Testing Exceptions in JUnit Tests
         By @Test(expected = NullPointerException.class)
Step 10 : Testing Performance in JUnit Tests
          By @Test(Timeout:1000); 10000 is in ms.
Step 11 : Parameterized Tests
          i) Add class level annotation:- @RunWith(Parameterized.class)
          ii) Define Actuals parameters b creating a static method with @Parameters which return Collection.
            like:- @Parameters
                    public static Collection<String[]> testConditions(){
                        String expectedOutput[][] = { {"AACD","CD"}, {"ACD","CD"} };  // can add any no of conditions
                        return Arrays.asList(expectedOutput);
                          }
          iii) Create two class level feilds input and expectedOutPut.
          iv)  Create Parameterized Constructor for these feilds.(eg:- AACD goes to input and CD goes to Output).
          v)    Instead of expected and actuals pass expectedOutPut and input.
Step 12 : Organize JUnits into Suites
        -Right click and choose junit-> choose Junit Test Suite--> Test Classes to inclcude in suite.
          A public Class is created with @RunWith(Suite.class) & @SuiteClasses({A.class, B.class})
