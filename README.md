Processing
==========

Syphon Implementation for Processing 2.0

INSTRUCTIONS

JSyphon package/Syphon Processing library build steps:

1) Write complementary java (in Eclipse) and Objective-C (in XCode) code, so that the Java classes 
have their methods implemented in native code in the .m file

2) Run the gen_headers script (in JSyphon/native_src) so the .h file is generated from the .class files that
Eclipse builds automatically

3) Build the jnlib native library from XCode (it will use the header generated in the previous step)

4) Run the ant build file of JSyphon from Eclipse, to generate jsyphon.jar

5) Copy the resulting jsyphon.jar (in JSyphon/distribution) and libJSyphon.jnilib (in JSyphon/native_libs) files to the lib folder of the Processing Syphon 
library project (and Syphon framework if it has changed)

6) Run ant build script for the Processing library.
