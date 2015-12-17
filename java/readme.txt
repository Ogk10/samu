If your lib can't find it to run:

1 navigate to you link-grammar folder.

2 create symbolic link
2.1 sudo ln -sv "$(pwd)/link-grammar/.libs/liblink-grammar.so.5" /usr/lib/
2.2 sudo ln -sv "$(pwd)/bindings/java-jni/.libs/liblink-grammar-java.so" /usr/lib/

2.3 If 2.1 & 2.2 already exist then delete them and repeat 2.1 & 2.2 else go to 3

3 navigate to the root of samu

4 compile with: javac -cp /YOUR LINK-GRAMMAR-X.Y.Z FOLDER ROOT/bindings/java/linkgrammar-X.Y.Z.jar *.java

5 run with: java -cp /YOUR LINK-GRAMMAR-X.Y.Z FOLDER ROOT/bindings/java/linkgrammar-X.Y.Z.jar:'pwd' Main
