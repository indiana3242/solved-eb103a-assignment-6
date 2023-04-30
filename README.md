Download Link: https://assignmentchef.com/product/solved-eb103a-assignment-6
<br>
<ul>

 <li>This is the first of two assignments dealing with SQL. Both assignments will use the same (or almost 62 the same) small database. This first assignment is simpler than the second one as this is the first 63 time you are actually writing and executing Oracle queries.</li>

 <li>2 Assignments</li>

 <li>(a) You are already supposed to know how to run SQL queries/commands on the Oracle 66 systems at CIMS. You were asked to familiarize yourself with and follow the instructions</li>

 <li>in How_To_Use_Oracle_At_CIMS.pdf.</li>

 <li>You were asked to do that earlier in order to save you time while working on this</li>

 <li></li>

 <li>So it is assumed that you know how to do that.</li>

 <li>(b) Look at the files ER06.drawio and relational06.architect. They will help 72 you understand the database schema defined in the files script06.sql and 73 sql. These files fully specify the application.</li>

</ul>

74 (c) Read script06.sql and dataSetupScript06.sql carefully. These scripts both define 75 and create the sample database and serves as the placeholder for putting in your solutions.

76 Look carefully over ANSWER0 there. It shows you how to insert a result of a query into 77 an empty table. It also uses the temp table TEMP0, just to demonstrate the usage of

<ul>

 <li>temp tables.</li>

 <li>(d) Input your queries into script06.sql after doing what is requested in Item 1e of Sec-</li>

 <li>tion 2.2.</li>

 <li>Please note which operations to use. Use only the operations that were introduced 82 in Unit 4 and the CREATE TABLE … AS …, used in the example of ANSWER0 in the</li>

 <li>So base your queries on the operations of selection, projection, cartesian product,</li>

 <li>minus, union, and intersection, with renaming and creation of new tables: creation, as 85 shown in the script. Do not, e.g., use JOINs of any kind. <em>To reiterate: A solution that </em>86      <em>used other operations (including those covered in Unit 5) will not be acceptable </em>87                In addition, use DISTINCT and ORDER BY as described below. If the output is to be 88         sorted in a different way, use an appropriate variant of ASC and DESC (ascending and</li>

 <li>descending) and list the sorting instructions in the appropriate order,</li>

 <li>For each query, <em>unless something else is required by the query </em>make sure to</li>

 <li>Remove duplicates from the answer (unless requested otherwise); that’s what DIS-</li>

 <li>TINCT does</li>

 <li>Sort the result in ascending order (unless requested otherwise); that’s what ORDER</li>

 <li>BY does</li>

 <li>This is <em>extremely important </em>to make the grading more manageable.</li>

 <li>So, for example, assuming that you are going to select a and b and rename b as c, you 97 should actually <em>explicitly </em>use:</li>

 <li>SELECT DISTINCT a, b AS c</li>

 <li>…</li>

 <li>ORDER BY a ASC, c ASC;</li>

 <li><em>Do not rely the on default removal of duplicates and sorting order. Add the </em>DISTINCT 102 <em>and </em>ORDER BY <em>instructions even if you think that they are not necessary.</em></li>

 <li>You may use temporary tables. If you choose to do that, use tables TEMP1, TEMP2,</li>

 <li>…, TEMP20.</li>

 <li>(e) Replace “zk1” in script06.sql with your NetID.</li>

 <li>(f) Do not remove the existing sample query.</li>

 <li>(g) Execute script06.sql, which internally calls dataSetupScript06.sql and produces a 108 spool file spool06.txt. The spool file must only include the details of the queries from 109                   sql. The spool file created will be a part of the submission.</li>

</ul>

110                  Do not be concerned that there are more placeholder ANSWERs, than the queries that 111                      you are supposed to produce.

112                  For reference, spool06.txt corresponding to the given script06.sql (with one sample 113       query) is enclosed.

114 The requested queries are listed below. Your answers must work for every 115 instance of the database and not only for the specific instance provided. The

116                  tables are named AnswerX, where “X” stands for the item number below. So, as the first 117                 item is item number 1, the first table is Answer1.

<ul>

 <li>Produce table AnswerX(RegNumber, TIN) that lists all the companies, sorted ascend-</li>

 <li>ing by RegNumber first and descending by TIN. Note that the order of the attributes 120 is not the same in both places.</li>

</ul>

121                  2. Produce table AnswerX(RegNumber, TIN) that lists all the big companies that work 122   in the ‘IT’ domain and are managed by people with familyName ‘Garcia’. 123            3. Produce table AnswerX(helperTIN, helpedTIN) that lists all the companies that help 124                each other. Note that (TIN1, TIN2) and (TIN2, TIN1) are not duplicates if TIN1 and

<ul>

 <li>TIN2 are not the same.</li>

 <li>Produce table AnswerX(RegNumber, TIN) that lists all the companies that work 127 in the ‘IT’ domain, and are helped by both companyOne with TIN ‘59515298’, and 128 companyTwo with TIN ‘51251930’.</li>

</ul>

129                  5. Produce table AnswerX(RegNumber, TIN) that lists all the companies (big or small) 130    that do not help any company.

<ul>

 <li>Produce table AnswerX(RegNumber, TIN) that lists all the companies, sorted as-</li>

 <li>cending by RegNumber first and ascending by TIN, that do not work in the ‘IT’</li>

 <li></li>

 <li>Produce table AnswerX(RegNumber, TIN) that lists all the small companies that work</li>

 <li>in ‘banking’ domain that work in the ‘IT’ domain, and are helped by small companies</li>

 <li>in ‘IT’ domain.</li>

 <li>3 What to submit</li>

 <li>Please upload 2 files, named <em>exactly </em>as specified and in the format <em>exactly </em>as specified.</li>

 <li>script06.sql, the script with your answers</li>

 <li>spool06.txt, the resulting spool file</li>

</ul>