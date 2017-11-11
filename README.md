# p4test
#include <iostream>
using namespace std;

#include "Shape.h"
#include "Circle.h"
#include "Rectangle.h"
#include "Line.h"
#include "Triangle.h"

#include "Color.h"
#include "Point.h"
#include "utility.h"
#include "Graphics.h"



void test_Point();
void test_Color();
void test_Circle();
void test_Line();
void test_Rectangle();
void test_Triangle();

int main(){
    test_Point();
    test_Color();
    test_Circle();
    test_Line();
    test_Rectangle();
    test_Triangle();
}

void test_Point(){
    //Point
    // test of default constructor
    Point p1;
    cout << p1 << endl;
    Point p2;
    Point p3;
    Point p4;
    Point p5;
    
    // test of the other constructor
    Point p(3, 9);
    cout << p << endl;
    
    // test of member function: setX()
    p1.setX(5);
    p2.setX(0);
    p3.setX(100);
    p4.setX(99);
    p5.setX(-1);
    // test of member function: setY()
    p1.setY(3);
    p2.setX(0);
    p3.setX(100);
    p4.setX(99);
    p5.setX(-1);
    
    // test of member functions getX() and getY()
    cout << "( " << p1.getX()
    << ", " << p1.getY()
    << " )" << endl;
    cout << "( " << p2.getX()
    << ", " << p2.getY()
    << " )" << endl;
    cout << "( " << p3.getX()
    << ", " << p3.getY()
    << " )" << endl;
    cout << "( " << p4.getX()
    << ", " << p4.getY()
    << " )" << endl;
    cout << "( " << p5.getX()
    << ", " << p5.getY()
    << " )" << endl;
    
    // you can also do cin >> p1;
    p1.read(cin);
    cout << p1 << endl;
}

void test_Color(){
    //Point
    // test of default constructor
    Color p11;
    cout << p11 << endl;
    Color p91;
    
    
    
    // test of the other constructor
    Color p(3, 9, 199);
    cout << p << endl;
    Color p21(255, 0, 0);
    Color p31(0, 0, 255);
    Color p41(0, 255, 0);
    Color p51(163, 9, 176);
    Color p61(163, 9, 176);
    Color p71(163, 9, 176);
    Color p81(0, 190, 225);
    
    
    
    // test of member function: setRed()
    p11.setRed(5);
    p21.setRed(0);
    p31.setRed(100);
    p41.setRed(99);
    p51.setRed(-1);
    p61.setRed(255);
    p71.setRed(256);
    p81.setRed(254);
    p91.setRed(1);
    
    // test of member function: setGreen()
    p11.setGreen(5);
    p21.setGreen(0);
    p31.setGreen(100);
    p41.setGreen(99);
    p51.setGreen(-1);
    p61.setGreen(255);
    p71.setGreen(256);
    p81.setGreen(210);
    p91.setGreen(1);
    
    // test of member function: setBlue()
    p11.setBlue(5);
    p21.setBlue(0);
    p31.setBlue(100);
    p41.setBlue(99);
    p51.setBlue(-1);
    p61.setBlue(255);
    p71.setBlue(256);
    p81.setBlue(15);
    p91.setBlue(1);
    
    
    // test of member functions getters
    cout << p11.getRed() << p11.getGreen()
    << p11.getBlue() << endl;
    cout << p21.getRed() << p21.getGreen()
    << p21.getBlue() << endl;
    cout << p31.getRed() << p31.getGreen()
    << p31.getBlue() << endl;
    cout << p41.getRed() << p41.getGreen()
    << p41.getBlue() << endl;
    cout << p51.getRed() << p51.getGreen()
    << p51.getBlue() << endl;
    cout << p61.getRed() << p61.getGreen()
    << p61.getBlue() << endl;
    cout << p71.getRed() << p71.getGreen()
    << p71.getBlue() << endl;
    cout << p81.getRed() << p81.getGreen()
    << p81.getBlue() << endl;
    cout << p91.getRed() << p91.getGreen()
    << p91.getBlue() << endl;
    
    
    
}
void test_Circle(){
    
    // test of default constructor
    Point pp2(23, 23);
    Point pp3(87, 10);
    Point pp4(78, 67);
    Point pp5(38, 35);
    
    Color cc2(25, 134, 43);
    Color cc3(25, 134, 43);
    Color cc4(25, 134, 43);
    Color cc5(25, 134, 43);
    
    Circle p13;
    Circle p23(pp2, 5, cc2);
    Circle p33(pp3, 13, cc3);
    Circle p43(pp4, 43, cc4);
    Circle p53(pp5, 2, cc5);
    
    cout << p13.getCenter() << p13.getRadius() << p13.getColor() << endl;
    cout << p23.getCenter() << p23.getRadius() << p23.getColor() << endl;
    cout << p33.getCenter() << p33.getRadius() << p33.getColor() << endl;
    cout << p43.getCenter() << p43.getRadius() << p43.getColor() << endl;
    cout << p53.getCenter() << p53.getRadius() << p53.getColor() << endl;
    
    Point pppp(23,6);
    Color pppc(23, 53, 234);
    // test of the other constructor
    Circle ppp(pppp, 5, pppc);
    cout << ppp.getCenter() << ppp.getRadius() << ppp.getColor() << endl;
    
    // test of member function: setCenter()
    Point a(5, 0);
    p13.setCenter(a);
    Point b(0, 0);
    p23.setCenter(b);
    Point c(100, 100);
    p33.setCenter(c);
    Point d(5, 0);
    p43.setCenter(d);
    Point e(67, 35);
    p53.setCenter(e);
    // test of member function: setRadius()
    p13.setRadius(3);
    p23.setRadius(0);
    p33.setRadius(100);
    p43.setRadius(99);
    p53.setRadius(-1);
    // test of member function: setColor()
    Color color1(0, 0, 0);
    p13.setColor(color1);
    Color color2(255, 0, 0);
    p23.setColor(color2);
    Color color3(0, 255, 0);
    p33.setColor(color3);
    Color color4(0, 0, 255);
    p43.setColor(color4);
    Color color5(255, 255, 255);
    p53.setColor(color4);
    Color color6(67, 2, 99);
    
    // test of member functions getX() and getY()
    cout << p13.getCenter() << p13.getRadius() << p13.getColor() << endl;
    cout << p23.getCenter() << p23.getRadius() << p23.getColor() << endl;
    cout << p33.getCenter() << p33.getRadius() << p33.getColor() << endl;
    cout << p43.getCenter() << p43.getRadius() << p43.getColor() << endl;
    cout << p53.getCenter() << p53.getRadius() << p53.getColor() << endl;
    
    
}


void test_Line(){
    // test of default constructor
    Point pp12(22, 34);
    Point pp13(26, 43);
    Point pp14(73, 35);
    Point pp15(34, 96);
    
    Point pp22(23, 34);
    Point pp23(28, 89);
    Point pp24(99, 5);
    Point pp25(2, 0);
    
    Color cc2(145, 45, 95);
    Color cc3(67, 243, 167);
    Color cc4(97, 45, 97);
    Color cc5(75, 55, 212);
    
    Line p13;
    Line p23(pp12, pp22, cc2);
    Line p33(pp13, pp23, cc3);
    Line p43(pp14, pp24, cc4);
    Line p53(pp15, pp25, cc5);
    cout << p13.getStart() << p13.getEnd() << p13.getColor() << endl;
    cout << p23.getStart() << p23.getEnd() << p23.getColor() << endl;
    cout << p33.getStart() << p33.getEnd() << p33.getColor() << endl;
    cout << p43.getStart() << p43.getEnd() << p43.getColor() << endl;
    cout << p53.getStart() << p53.getEnd() << p53.getColor() << endl;
    
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    
    // test of the other constructor
    Point ppps(24, 34);
    Point pppe(57, 96);
    Color pppc(234, 56, 99);
    Line ppp(ppps, pppe, pppc);
    cout << ppp.getStart() << ppp.getEnd() << ppp.getColor() << endl;
    
    // test of member function: setCenter()
    Point a(5, 0);
    p13.setStart(a);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point b(0, 0);
    p23.setStart(b);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point c(100, 100);
    p33.setStart(c);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point d(5, 0);
    p43.setStart(d);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point e(67, 35);
    p53.setStart(e);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    // test of member function: setRadius()
    Point a1(15, 6);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    p13.setEnd(a1);
    Point b1(4, 27);
    p23.setEnd(b1);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point c1(100, 100);
    p33.setEnd(c1);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point d1(5, 7);
    p43.setEnd(d1);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Point e1(67, 34);
    p53.setEnd(e1);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    // test of member function: setColor()
    Color color1(0, 0, 0);
    p13.setColor(color1);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Color color2(255, 0, 0);
    p23.setColor(color2);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Color color3(0, 255, 0);
    p33.setColor(color3);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Color color4(0, 0, 255);
    p43.setColor(color4);
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    Color color5(255, 255, 255);
    p53.setColor(color5);
    Color color6(67, 2, 99);
    
    // test of member functions getX() and getY()
    cout << p13.getStart() << p13.getEnd() << p13.getColor() << endl;
    cout << p23.getStart() << p23.getEnd() << p23.getColor() << endl;
    cout << p33.getStart() << p33.getEnd() << p33.getColor() << endl;
    cout << p43.getStart() << p43.getEnd() << p43.getColor() << endl;
    cout << p53.getStart() << p53.getEnd() << p53.getColor() << endl;
    
    p13.write(cout);
    p23.write(cout);
    p33.write(cout);
    p43.write(cout);
    p53.write(cout);
    
}

void test_Rectangle(){
    
    Rectangle r1;
    cout << r1.getStart() << r1.getEnd() << r1.getColorTopLeft() << r1.getColorTopRight() << r1.getColorBottomRight() << r1.getColorBottomLeft();
    
    Point v11(20,0);
    Point v21(21,2);
    Color c01(120, 20, 103);
    Color c11(160, 20, 103);
    Color c21(157, 130, 250);
    Color c31(43, 170, 230);
    
    Rectangle r2(v11, v21, c01);
    cout << r2.getStart() << r2.getEnd() << r2.getColorTopLeft() << r2.getColorTopRight() << r2.getColorBottomRight() << r2.getColorBottomLeft();
    
    Rectangle t1(v11, v21, c01, c11, c21, c31);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    Point v42(94,93);
    Point v43(93,39);
    Point v44(27,35);
    Point v45(1,66);
    Point v46(47,65);
    
    Point v41(0,0);
    Point v51(1,2);
    Color c71(100, 100, 100);
    Color c41(100, 100, 100);
    Color c51(150, 150, 150);
    Color c61(50, 100, 150);
    
    Color c81(34, 76, 278);
    Color c82(24, 154, 145);
    Color c83(4, 65, 67);
    Color c84(37, 43, 265);
    Color c85(234, 78, 234);
    
    t1.setStart(v41);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setStart(v42);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setStart(v43);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setStart(v44);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setStart(v45);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setStart(v46);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setEnd(v51);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColor(c81);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColor(c82);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColor(c83);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColor(c84);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColor(c85);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColorTopLeft(c71);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColorTopRight(c41);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColorBottomRight(c51);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
    t1.setColorBottomLeft(c61);
    cout << t1.getStart() << t1.getEnd() << t1.getColorTopLeft() << t1.getColorTopRight() << t1.getColorBottomRight() << t1.getColorBottomLeft();
    
}


void test_Triangle(){
    
    Point v11(20,0);
    Point v21(20,2);
    Point v31(11,15);
    Color c11(160, 20, 103);
    Color c21(157, 130, 250);
    Color c31(43, 170, 230);
    
    Triangle t1(v11, c11, v21, c21, v31, c31);
    t1.write(cout);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    
    Point v41(0,0);
    Point v51(0,2);
    Point v61(1,1);
    Color c41(100, 100, 100);
    Color c51(150, 150, 150);
    Color c61(50, 100, 150);
    
    t1.setVertexOne(v41);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
    t1.setVertexTwo(v51);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
    t1.setVertexThree(v61);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
    t1.setVertexOneColor(c41);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
    t1.setVertexTwoColor(c51);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
    t1.setVertexThreeColor(c61);
    cout << t1.getVertexOne() << t1.getVertexTwo() << t1.getVertexThree() << t1.getVertexOneColor() << t1.getVertexTwoColor() << t1.getVertexThreeColor();
    t1.write(cout);
    
}
