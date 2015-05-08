<h2>Data Loading Examples</h2>

Some examples of loading data into an Oracle database, and note that the Java code includes examples of both good and (very!) bad practice. For full details, and the background behind the examples, check out the <a href="https://www.youtube.com/watch?v=Tr2DC-1W0i8&feature=youtu.be">Youtube web seminar.</a>. The seminar will explain how you can ensure that your data load code will enable your application to scale as your data volumes and load rates increase.

The Java was tested on JDK 7 and Oracle Database 12.1.0.2, but it will work without issue on Oracle 11gR2 too. To compile it, your project will need to include the Oracle JDBC client libraries.

The Python example requires <a href="http://cx-oracle.sourceforge.net/">cx_Oracle</a>, which in turn depends an Oracle client installation (for example, the <a href="http://www.oracle.com/technetwork/database/features/instant-client/index.html">basic instant client plus the SDK).</a>

The <a href="https://github.com/oracle/dw-vldb/blob/master/db_load/example_output.txt">example output file</a> is included so that you can see how the Java code behaves. Note that it shows what happens if you use a transatlantic SQLNet connection: any optimization that reduces the number of network rountrips results in a very significant performance improvment - above all others! If you are using a local database, you will want to increase *rowCount* significantly.