CC = g++
CFLAGS = -lssl -lcrypto -lm

rec:main.o receiver.o sha256.o
	$(CC) -o rec main.o receiver.o sha256.o $(CFLAGS)
main.o:main.cpp
	$(CC) -c main.cpp $(CFLAGS)
receiver.o:receiver.cpp
	$(CC) -c receiver.cpp $(CFLAGS)
sha256.o:sha256.cpp
	$(CC) -c sha256.cpp $(CFLAGS)

clean:
	rm rec main.o receiver.o sha256.o
