# IDcard Recognization
the project contains 4 modules:
* rectangle deskew -> dir deskew
* textline detection -> dir detect/ 
* textline recognization -> dir textline/
* classify engine(needed by textline recognization) -> dir deep_engine/
* a interface to call -> dir idcardrec/

note: Detection is not included here, see CTPN

## build
mkdir build && cd build && cmake .. && make

## improvement
In this version, the deskew code is commented in idcardrec/src/IDcardReader.cpp, Line 28.
So the test image is a textline image instead of a ID card.
When the detection codes finished, you can uncomment the deskew, and use a ID card image as input.
