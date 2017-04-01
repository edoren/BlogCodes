all: LoadLibrary

clean:
	rm libHelloLibrary.so LoadLibrary.bin

HelloLibrary: HelloLibrary.cpp
	g++ HelloLibrary.cpp -o libHelloLibrary.so -shared -fPIC

LoadLibrary: HelloLibrary LoadLibrary.cpp
	g++ -std=c++11 LoadLibrary.cpp -o LoadLibrary.bin -ldl

