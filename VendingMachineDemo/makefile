
VendingMachineTest : VendingMachineTestMain.o VendingMachine.o Item.o
	g++ -std=c++11 VendingMachineTestMain.o VendingMachine.o Item.o -lgtest -lgtest_main -pthread -o VendingMachineTest

VendingMachineTestMain.o : VendingMachineTestMain.cpp Item.hpp VendingMachine.hpp
	g++ -std=c++11 -c VendingMachineTestMain.cpp
	
Item.o : Item.cpp Item.hpp
	g++ -std=c++11 -c Item.cpp

VendingMachine.o : VendingMachine.cpp VendingMachine.hpp Item.hpp
	g++ -std=c++11 -c VendingMachine.cpp

clean :
	rm VendingMachineTest VendingMachineTestMain.o VendingMachine.o Item.o
