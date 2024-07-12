# hadoop-examples-mapreduce

- Clone the project.
    ```bash
    git clone https://github.com/makayel/hadoop-examples-mapreduce.git
    ```
    ```bash
    cd hadoop-examples-mapreduces
    ```

- Start by installing OpenJDK 8.    
    ```bash
    brew tap AdoptOpenJDK/openjdk
    ```
    ```bash
    brew install --cask adoptopenjdk8
    ```
    
- Then install maven.
    
    ```bash
    brew install maven
    ```

- Modify the [pom.xml](./pom.xml) file 

- Run the following Maven command to build your project.
    ```bash
    mvn clean
    [INFO] Scanning for projects...
    [INFO]
    [INFO] ----------------< com.opstty:hadoop-examples-mapreduce >----------------
    [INFO] Building hadoop-examples-mapreduce 1.0-SNAPSHOT
    [INFO]   from pom.xml
    [INFO] --------------------------------[ jar ]---------------------------------
    [INFO]
    [INFO] --- clean:3.2.0:clean (default-clean) @ hadoop-examples-mapreduce ---
    [INFO] Deleting /Users/wandrille/Desktop/hadoop-examples-mapreduce/target
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time:  0.475 s
    [INFO] Finished at: 2024-07-12T10:39:10+02:00
    [INFO] ------------------------------------------------------------------------
    ```
    ```bash
    mvn package
    [INFO] Scanning for projects...
    [INFO]
    [INFO] ----------------< com.opstty:hadoop-examples-mapreduce >----------------
    [INFO] Building hadoop-examples-mapreduce 1.0-SNAPSHOT
    [INFO]   from pom.xml
    [INFO] --------------------------------[ jar ]---------------------------------
    [WARNING] 2 problems were encountered while building the effective model for org.apache.yetus:audience-annotations:jar:0.5.0
    [INFO]
    [INFO] --- resources:3.3.1:resources (default-resources) @ hadoop-examples-mapreduce ---
    [INFO] skip non existing resourceDirectory /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/main/resources
    [INFO]
    [INFO] --- compiler:3.8.1:compile (default-compile) @ hadoop-examples-mapreduce ---
    [INFO] Changes detected - recompiling the module!
    [INFO] Compiling 4 source files to /Users/wandrille/Desktop/hadoop-examples-mapreduce/target/classes
    [INFO]
    [INFO] --- resources:3.3.1:testResources (default-testResources) @ hadoop-examples-mapreduce ---
    [INFO] Copying 1 resource from src/test/resources to target/test-classes
    [INFO]
    [INFO] --- compiler:3.8.1:testCompile (default-testCompile) @ hadoop-examples-mapreduce ---
    [INFO] Changes detected - recompiling the module!
    [INFO] Compiling 2 source files to /Users/wandrille/Desktop/hadoop-examples-mapreduce/target/test-classes
    [INFO] /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/test/java/com/opstty/reducer/IntSumReducerTest.java: Some input files use or override a deprecated API.
    [INFO] /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/test/java/com/opstty/reducer/IntSumReducerTest.java: Recompile with -Xlint:deprecation for details.
    [INFO] /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/test/java/com/opstty/reducer/IntSumReducerTest.java: Some input files use unchecked or unsafe operations.
    [INFO] /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/test/java/com/opstty/reducer/IntSumReducerTest.java: Recompile with -Xlint:unchecked for details.
    [INFO]
    [INFO] --- surefire:3.2.5:test (default-test) @ hadoop-examples-mapreduce ---
    [INFO] Using auto detected provider org.apache.maven.surefire.junit4.JUnit4Provider
    [INFO]
    [INFO] -------------------------------------------------------
    [INFO]  T E S T S
    [INFO] -------------------------------------------------------
    [INFO] Running com.opstty.mapper.TokenizerMapperTest
    [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.936 s -- in com.opstty.mapper.TokenizerMapperTest
    [INFO] Running com.opstty.reducer.IntSumReducerTest
    [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.011 s -- in com.opstty.reducer.IntSumReducerTest
    [INFO]
    [INFO] Results:
    [INFO]
    [INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0
    [INFO]
    [INFO]
    [INFO] --- jar:3.4.1:jar (default-jar) @ hadoop-examples-mapreduce ---
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.1.0/file-management-3.1.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.1.0/file-management-3.1.0.pom (4.5 kB at 6.0 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/36/maven-shared-components-36.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/36/maven-shared-components-36.pom (4.9 kB at 175 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/36/maven-parent-36.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/36/maven-parent-36.pom (45 kB at 568 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/26/apache-26.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/26/apache-26.pom (21 kB at 133 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.1/plexus-utils-4.0.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.1/plexus-utils-4.0.1.pom (7.8 kB at 72 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/17/plexus-17.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/17/plexus-17.pom (28 kB at 705 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.16.1/commons-io-2.16.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.16.1/commons-io-2.16.1.pom (20 kB at 892 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/69/commons-parent-69.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/69/commons-parent-69.pom (77 kB at 1.9 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.2/maven-archiver-3.6.2.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.2/maven-archiver-3.6.2.pom (4.4 kB at 244 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/41/maven-shared-components-41.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/41/maven-shared-components-41.pom (3.2 kB at 176 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.9.2/plexus-archiver-4.9.2.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.9.2/plexus-archiver-4.9.2.pom (6.0 kB at 333 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.2/plexus-io-3.4.2.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.2/plexus-io-3.4.2.pom (3.9 kB at 257 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/16/plexus-16.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/16/plexus-16.pom (28 kB at 1.4 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.26.1/commons-compress-1.26.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.26.1/commons-compress-1.26.1.pom (22 kB at 895 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/66/commons-parent-66.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/66/commons-parent-66.pom (77 kB at 2.6 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.16.1/commons-codec-1.16.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.16.1/commons-codec-1.16.1.pom (16 kB at 922 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.14.0/commons-lang3-3.14.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.14.0/commons-lang3-3.14.0.pom (31 kB at 180 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/64/commons-parent-64.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/64/commons-parent-64.pom (78 kB at 1.2 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/30/apache-30.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/30/apache-30.pom (23 kB at 1.2 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.pom (15 kB at 969 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.9/xz-1.9.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.9/xz-1.9.pom (2.0 kB at 58 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-11/zstd-jni-1.5.5-11.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-11/zstd-jni-1.5.5-11.pom (2.0 kB at 118 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.27/plexus-interpolation-1.27.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.27/plexus-interpolation-1.27.pom (3.0 kB at 178 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.1.0/file-management-3.1.0.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/file-management/3.1.0/file-management-3.1.0.jar (36 kB at 1.5 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.16.1/commons-io-2.16.1.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.2/maven-archiver-3.6.2.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.27/plexus-interpolation-1.27.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.1/plexus-utils-4.0.1.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.9.2/plexus-archiver-4.9.2.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.2/maven-archiver-3.6.2.jar (27 kB at 865 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.2/plexus-io-3.4.2.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.2/plexus-io-3.4.2.jar (79 kB at 249 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.26.1/commons-compress-1.26.1.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-interpolation/1.27/plexus-interpolation-1.27.jar (86 kB at 169 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.14.0/commons-lang3-3.14.0.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.1/plexus-utils-4.0.1.jar (193 kB at 308 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.16.1/commons-codec-1.16.1.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.9.2/plexus-archiver-4.9.2.jar (225 kB at 200 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.16.1/commons-io-2.16.1.jar (509 kB at 303 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.9/xz-1.9.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/iq80/snappy/snappy/0.4/snappy-0.4.jar (58 kB at 29 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-11/zstd-jni-1.5.5-11.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/tukaani/xz/1.9/xz-1.9.jar (116 kB at 44 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/commons-codec/commons-codec/1.16.1/commons-codec-1.16.1.jar (365 kB at 138 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.26.1/commons-compress-1.26.1.jar (1.1 MB at 400 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-lang3/3.14.0/commons-lang3-3.14.0.jar (658 kB at 181 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-11/zstd-jni-1.5.5-11.jar (6.8 MB at 715 kB/s)
    [INFO] Building jar: /Users/wandrille/Desktop/hadoop-examples-mapreduce/target/hadoop-examples-mapreduce-1.0-SNAPSHOT.jar
    [INFO]
    [INFO] --- assembly:3.7.1:single (default) @ hadoop-examples-mapreduce ---
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.pom (2.8 kB at 175 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver/1.4.1/maven-resolver-1.4.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver/1.4.1/maven-resolver-1.4.1.pom (18 kB at 826 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.pom (2.6 kB at 164 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.3.2/maven-common-artifact-filters-3.3.2.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.3.2/maven-common-artifact-filters-3.3.2.pom (5.3 kB at 30 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/37/maven-shared-components-37.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/37/maven-shared-components-37.pom (4.9 kB at 163 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/37/maven-parent-37.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/37/maven-parent-37.pom (46 kB at 2.1 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/apache/27/apache-27.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/apache/27/apache-27.pom (20 kB at 970 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/3.3.2/maven-filtering-3.3.2.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/3.3.2/maven-filtering-3.3.2.pom (31 kB at 1.7 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-xml/3.0.0/plexus-xml-3.0.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-xml/3.0.0/plexus-xml-3.0.0.pom (3.7 kB at 288 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.1/maven-archiver-3.6.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.1/maven-archiver-3.6.1.pom (4.1 kB at 113 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/40/maven-shared-components-40.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-shared-components/40/maven-shared-components-40.pom (3.2 kB at 107 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/40/maven-parent-40.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-parent/40/maven-parent-40.pom (49 kB at 1.4 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.8.0/plexus-archiver-4.8.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-archiver/4.8.0/plexus-archiver-4.8.0.pom (6.1 kB at 469 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/14/plexus-14.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus/14/plexus-14.pom (28 kB at 201 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.1/plexus-io-3.4.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-io/3.4.1/plexus-io-3.4.1.pom (6.0 kB at 62 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.13.0/commons-io-2.13.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/commons-io/commons-io/2.13.0/commons-io-2.13.0.pom (20 kB at 813 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/58/commons-parent-58.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/58/commons-parent-58.pom (83 kB at 1.6 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.23.0/commons-compress-1.23.0.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-compress/1.23.0/commons-compress-1.23.0.pom (22 kB at 625 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/56/commons-parent-56.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/commons/commons-parent/56/commons-parent-56.pom (82 kB at 2.4 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/junit/junit-bom/5.9.1/junit-bom-5.9.1.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/org/junit/junit-bom/5.9.1/junit-bom-5.9.1.pom (5.6 kB at 512 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-5/zstd-jni-1.5.5-5.pom
    Downloaded from central: https://repo.maven.apache.org/maven2/com/github/luben/zstd-jni/1.5.5-5/zstd-jni-1.5.5-5.pom (1.9 kB at 128 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-util/1.4.1/maven-resolver-util-1.4.1.jar (168 kB at 2.5 MB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.3.2/maven-common-artifact-filters-3.3.2.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/3.3.2/maven-filtering-3.3.2.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.1/maven-archiver-3.6.1.jar
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.0/plexus-utils-4.0.0.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-common-artifact-filters/3.3.2/maven-common-artifact-filters-3.3.2.jar (58 kB at 655 kB/s)
    Downloading from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-xml/3.0.0/plexus-xml-3.0.0.jar
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/resolver/maven-resolver-api/1.4.1/maven-resolver-api-1.4.1.jar (149 kB at 1.7 MB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/shared/maven-filtering/3.3.2/maven-filtering-3.3.2.jar (56 kB at 220 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/apache/maven/maven-archiver/3.6.1/maven-archiver-3.6.1.jar (27 kB at 103 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-utils/4.0.0/plexus-utils-4.0.0.jar (192 kB at 192 kB/s)
    Downloaded from central: https://repo.maven.apache.org/maven2/org/codehaus/plexus/plexus-xml/3.0.0/plexus-xml-3.0.0.jar (93 kB at 86 kB/s)
    [INFO] Building jar: /Users/wandrille/Desktop/hadoop-examples-mapreduce/target/hadoop-examples-mapreduce-1.0-SNAPSHOT-jar-with-dependencies.jar
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time:  33.137 s
    [INFO] Finished at: 2024-07-12T10:39:51+02:00
    [INFO] ------------------------------------------------------------------------
    ```
    ```bash
    mvn test
    [INFO] Scanning for projects...
    [INFO]
    [INFO] ----------------< com.opstty:hadoop-examples-mapreduce >----------------
    [INFO] Building hadoop-examples-mapreduce 1.0-SNAPSHOT
    [INFO]   from pom.xml
    [INFO] --------------------------------[ jar ]---------------------------------
    [WARNING] 2 problems were encountered while building the effective model for org.apache.yetus:audience-annotations:jar:0.5.0
    [INFO]
    [INFO] --- resources:3.3.1:resources (default-resources) @ hadoop-examples-mapreduce ---
    [INFO] skip non existing resourceDirectory /Users/wandrille/Desktop/hadoop-examples-mapreduce/src/main/resources
    [INFO]
    [INFO] --- compiler:3.8.1:compile (default-compile) @ hadoop-examples-mapreduce ---
    [INFO] Nothing to compile - all classes are up to date
    [INFO]
    [INFO] --- resources:3.3.1:testResources (default-testResources) @ hadoop-examples-mapreduce ---
    [INFO] Copying 1 resource from src/test/resources to target/test-classes
    [INFO]
    [INFO] --- compiler:3.8.1:testCompile (default-testCompile) @ hadoop-examples-mapreduce ---
    [INFO] Nothing to compile - all classes are up to date
    [INFO]
    [INFO] --- surefire:3.2.5:test (default-test) @ hadoop-examples-mapreduce ---
    [INFO] Using auto detected provider org.apache.maven.surefire.junit4.JUnit4Provider
    [INFO]
    [INFO] -------------------------------------------------------
    [INFO]  T E S T S
    [INFO] -------------------------------------------------------
    [INFO] Running com.opstty.mapper.TokenizerMapperTest
    [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.907 s -- in com.opstty.mapper.TokenizerMapperTest
    [INFO] Running com.opstty.reducer.IntSumReducerTest
    [INFO] Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.057 s -- in com.opstty.reducer.IntSumReducerTest
    [INFO]
    [INFO] Results:
    [INFO]
    [INFO] Tests run: 2, Failures: 0, Errors: 0, Skipped: 0
    [INFO]
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time:  3.662 s
    [INFO] Finished at: 2024-07-12T10:39:58+02:00
    [INFO] ------------------------------------------------------------------------
    ```

- Send the JAR to the edge node.
        
    ```bash
    scp /Users/wandrille/Desktop/hadoop-examples-mapreduce/target/hadoop-examples-mapreduce-1.0-SNAPSHOT.jar wandrille.dioubate@bigdata01.efrei.hadoop.clemlab.io:/home/wandrille.dioubate/
    wandrille.dioubate@bigdata01.efrei.hadoop.clemlab.io's password:
    hadoop-examples-mapreduce-1.0-SNAPSHOT.jar                                              100% 6714    33.7KB/s   00:00
    ```
        
    
- Connexion to cluster
    
    ```bash
    ssh wandrille.dioubate@bigdata01.efrei.hadoop.clemlab.io
    wandrille.dioubate@bigdata01.efrei.hadoop.clemlab.io's password:
    ```
    ```bash
    cd /home
    ```
    ```bash
    cd wandrille.dioubate/
    ```
    ```bash
    ls
    hadoop-examples-mapreduce-1.0-SNAPSHOT.jar  input.txt
    ```

- Run wordcount job. 
    - Create input file.
    ```bash
    hdfs dfs -mkdir -p input
    ```
    ```bash
    echo "Hello Hadoop Hello MapReduce" > input.txt
    ```
    ```bash
    hdfs dfs -put input.txt /user/wandrille.dioubate/input/
    ```
    - Run the wordcount job
    ```bash
    hadoop jar hadoop-examples-mapreduce-1.0-SNAPSHOT.jar com.opstty.job.WordCount /user/wandrille.dioubate/input /user/wandrille.dioubate/output
    24/07/12 11:04:49 INFO client.AHSProxy: Connecting to Application History server at bigdata02.efrei.hadoop.clemlab.io/62.210.145.80:10200
    24/07/12 11:04:49 INFO hdfs.DFSClient: Created token for wandrille.dioubate: HDFS_DELEGATION_TOKEN owner=wandrille.dioubate@EFREI.HADOOP.CLEMLAB.IO, renewer=yarn, realUser=, issueDate=1720775089237, maxDate=1721379889237, sequenceNumber=908, masterKeyId=17 on ha-hdfs:efrei
    24/07/12 11:04:49 INFO kms.KMSClientProvider: New token created: (Kind: kms-dt, Service: kms://http@bigdata03.efrei.hadoop.clemlab.io:9292/kms, Ident: (kms-dt owner=wandrille.dioubate, renewer=yarn, realUser=, issueDate=1720775089293, maxDate=1721379889293, sequenceNumber=807, masterKeyId=5))
    24/07/12 11:04:49 INFO security.TokenCache: Got dt for hdfs://efrei; Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:efrei, Ident: (token for wandrille.dioubate: HDFS_DELEGATION_TOKEN owner=wandrille.dioubate@EFREI.HADOOP.CLEMLAB.IO, renewer=yarn, realUser=, issueDate=1720775089237, maxDate=1721379889237, sequenceNumber=908, masterKeyId=17)
    24/07/12 11:04:49 INFO security.TokenCache: Got dt for hdfs://efrei; Kind: kms-dt, Service: kms://http@bigdata03.efrei.hadoop.clemlab.io:9292/kms, Ident: (kms-dt owner=wandrille.dioubate, renewer=yarn, realUser=, issueDate=1720775089293, maxDate=1721379889293, sequenceNumber=807, masterKeyId=5)
    24/07/12 11:04:49 INFO mapreduce.JobResourceUploader: Disabling Erasure Coding for path: /user/wandrille.dioubate/.staging/job_1720701352744_0342
    24/07/12 11:04:49 INFO input.FileInputFormat: Total input files to process : 1
    24/07/12 11:04:49 INFO mapreduce.JobSubmitter: number of splits:1
    24/07/12 11:04:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1720701352744_0342
    24/07/12 11:04:49 INFO mapreduce.JobSubmitter: Executing with tokens: [Kind: kms-dt, Service: kms://http@bigdata03.efrei.hadoop.clemlab.io:9292/kms, Ident: (kms-dt owner=wandrille.dioubate, renewer=yarn, realUser=, issueDate=1720775089293, maxDate=1721379889293, sequenceNumber=807, masterKeyId=5), Kind: HDFS_DELEGATION_TOKEN, Service: ha-hdfs:efrei, Ident: (token for wandrille.dioubate: HDFS_DELEGATION_TOKEN owner=wandrille.dioubate@EFREI.HADOOP.CLEMLAB.IO, renewer=yarn, realUser=, issueDate=1720775089237, maxDate=1721379889237, sequenceNumber=908, masterKeyId=17)]
    24/07/12 11:04:49 INFO conf.Configuration: found resource resource-types.xml at file:/etc/hadoop/1.2.4.0-10/0/resource-types.xml
    24/07/12 11:04:49 INFO impl.TimelineClientImpl: Timeline service address: bigdata02.efrei.hadoop.clemlab.io:8190
    24/07/12 11:04:50 INFO impl.YarnClientImpl: Submitted application application_1720701352744_0342
    24/07/12 11:04:50 INFO mapreduce.Job: The url to track the job: https://bigdata01.efrei.hadoop.clemlab.io:8090/proxy/application_1720701352744_0342/
    24/07/12 11:04:50 INFO mapreduce.Job: Running job: job_1720701352744_0342
    24/07/12 11:04:56 INFO mapreduce.Job: Job job_1720701352744_0342 running in uber mode : false
    24/07/12 11:04:56 INFO mapreduce.Job:  map 0% reduce 0%
    24/07/12 11:05:00 INFO mapreduce.Job:  map 100% reduce 0%
    24/07/12 11:05:04 INFO mapreduce.Job:  map 100% reduce 100%
    24/07/12 11:05:04 INFO mapreduce.Job: Job job_1720701352744_0342 completed successfully
    24/07/12 11:05:04 INFO mapreduce.Job: Counters: 54
        File System Counters
            FILE: Number of bytes read=47
            FILE: Number of bytes written=612573
            FILE: Number of read operations=0
            FILE: Number of large read operations=0
            FILE: Number of write operations=0
            HDFS: Number of bytes read=146
            HDFS: Number of bytes written=29
            HDFS: Number of read operations=8
            HDFS: Number of large read operations=0
            HDFS: Number of write operations=2
            HDFS: Number of bytes read erasure-coded=0
        Job Counters
            Launched map tasks=1
            Launched reduce tasks=1
            Data-local map tasks=1
            Total time spent by all maps in occupied slots (ms)=7974
            Total time spent by all reduces in occupied slots (ms)=5476
            Total time spent by all map tasks (ms)=2658
            Total time spent by all reduce tasks (ms)=1369
            Total vcore-milliseconds taken by all map tasks=2658
            Total vcore-milliseconds taken by all reduce tasks=1369
            Total megabyte-milliseconds taken by all map tasks=4082688
            Total megabyte-milliseconds taken by all reduce tasks=2803712
        Map-Reduce Framework
            Map input records=1
            Map output records=4
            Map output bytes=45
            Map output materialized bytes=47
            Input split bytes=117
            Combine input records=4
            Combine output records=3
            Reduce input groups=3
            Reduce shuffle bytes=47
            Reduce input records=3
            Reduce output records=3
            Spilled Records=6
            Shuffled Maps =1
            Failed Shuffles=0
            Merged Map outputs=1
            GC time elapsed (ms)=61
            CPU time spent (ms)=1040
            Physical memory (bytes) snapshot=1523822592
            Virtual memory (bytes) snapshot=6695829504
            Total committed heap usage (bytes)=1521483776
            Peak Map Physical memory (bytes)=1192189952
            Peak Map Virtual memory (bytes)=3108732928
            Peak Reduce Physical memory (bytes)=331632640
            Peak Reduce Virtual memory (bytes)=3587096576
        Shuffle Errors
            BAD_ID=0
            CONNECTION=0
            IO_ERROR=0
            WRONG_LENGTH=0
            WRONG_MAP=0
            WRONG_REDUCE=0
        File Input Format Counters
            Bytes Read=29
        File Output Format Counters
            Bytes Written=29
    ```
