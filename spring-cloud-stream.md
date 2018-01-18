

1.  dummy
    ```
    The @EnableBinding annotation takes one or more interfaces as parameters (in this case, the parameter is a single Sink interface). An interface declares input and/or output channels. Spring Cloud Stream provides the interfaces Source, Sink, and Processor; you can also define your own interfaces.
    
    The following is the definition of the Sink interface:
    
    public interface Sink {
      String INPUT = "input";
    
      @Input(Sink.INPUT)
      SubscribableChannel input();
    }
    The @Input annotation identifies an input channel, through which received messages enter the application; the @Output annotation identifies an output channel, through which published messages leave the application. The @Input and @Output annotations can take a channel name as a parameter; if a name is not provided, the name of the annotated method will be used.

    Spring Cloud Stream will create an implementation of the interface for you. You can use this in the application by autowiring it, as in the following example of a test case.
    
    @RunWith(SpringJUnit4ClassRunner.class)
    @SpringApplicationConfiguration(classes = VoteRecordingSinkApplication.class)
    @WebAppConfiguration
    @DirtiesContext
    public class StreamApplicationTests {
    
      @Autowired
      private Sink sink;
    
      @Test
      public void contextLoads() {
        assertNotNull(this.sink.input());
      }
    }
    ```


1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```

1.  dymmy
    ```
    ```



