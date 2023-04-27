## Environment:

```
JDK: Java 8 or more
Source load: JMeter 5.0 or more
```

## Run tests

 1. Download [Apache JMeter 5.5](https://jmeter.apache.org/download_jmeter.cgi) (Requires Java 8+) extract it to a convenient folder.

 2. Run cmd from ```apache-jmeter-5.5/bin``` directory.
 3. Run the test with correct project root path. Before run the test you should delete result.csv and report folder from the root of the project.
    * Load test
              
          jmeter -Jusers=3 -JrampUp=30 -Jduration=60 -n -t <*root path to project*>/594712/DemoBlaze-1.0.0.jmx -l <*root path to project*>/594712/result.csv -e -o <*root path to project*>/594712/report/
		  
## Test report
Test result.csv and Jmeter report will be generated in the project folder:
 * result.csv: ```/594712/```
 * Jmeter report: ```/594712/report/```