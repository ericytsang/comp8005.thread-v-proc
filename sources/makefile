
CC = g++ -Wall -W -Wextra -pedantic -g
LIBS = -lgmp -lpthread



clean:
	rm -f *.o *.out



# executables
Processes-Main: Processes-Main.o FindFactorsTask.o
	$(CC) -o ./Processes-Main.out Processes-Main.o FindFactorsTask.o $(LIBS)

Threads-Main: Threads-Main.o FindFactorsTask.o Number.o
	$(CC) -o ./Threads-Main.out Threads-Main.o FindFactorsTask.o Number.o $(LIBS)

FindFactorsTaskTest: FindFactorsTaskTest.o FindFactorsTask.o Number.o
	$(CC) -o ./FindFactorsTaskTest.out FindFactorsTaskTest.o FindFactorsTask.o Number.o $(LIBS)

NumberTest: NumberTest.o Number.o
	$(CC) -o ./NumberTest.out NumberTest.o Number.o $(LIBS)

# files
Threads-Main.o: Threads-Main.cpp
	$(CC) -c Threads-Main.cpp

Processes-Main.o: Processes-Main.cpp
	$(CC) -c Processes-Main.cpp

FindFactorsTaskTest.o: FindFactorsTaskTest.cpp
	$(CC) -c FindFactorsTaskTest.cpp

FindFactorsTask.o: FindFactorsTask.cpp
	$(CC) -c FindFactorsTask.cpp

Number.o: Number.cpp
	$(CC) -c Number.cpp