# p4test
void test_point();
void test_Color();
void test_Graphics();
void test_pics();
void test_Circle();
void test_Line();
void test_Rectangle();
void test_Shape();
void test_Triangle();

int main(){
    test_point();
    test_Color();
    test_Graphics();
    test_pics();
    test_Circle();
    test_Line();
    test_Rectangle();
    test_Shape();
    test_Triangle();
}

void test_point(){
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
    cout << p1 << endl;
    
   
    
    // test of the other constructor
    Point p(3, 9, 199);
    cout << p << endl;
    Point p21(255, 0, 0);
    Point p31(0, 0, 255);
    Point p41(0, 255, 0);
    Point p51(163, 9, 176);
 
    
    
    // test of member function: setRed()
    p11.setRed(5);
    p21.setRed(0);
    p31.setRed(100);
    p41.setRed(99);
    p51.setRed(-1);
    p61.setRed(255);
    p71.setRed(256);
    
    // test of member function: setGreen()
    p11.setGreen(5);
    p21.setGreen(0);
    p31.setGreen(100);
    p41.setGreen99);
    p51.setGreen(-1);
    p61.setGreen(255);
    p71.setGreen(256);
    
    // test of member function: setBlue()
    p11.setBlue(5);
    p21.setBlue(0);
    p31.setBlue(100);
    p41.setBlue(99);
    p51.setBlue(-1);
    p61.setBlue(255);
    p71.setBlue(256);
  
    
    // test of member functions getters
    cout << p11.getRed() << p11.getGreen()
    << p11.getGreen() << endl;
     cout << p21.getRed() << p21.getGreen()
    << p21.getGreen() << endl;
     cout << p31.getRed() << p31.getGreen()
    << p31.getGreen() << endl;
     cout << p41.getRed() << p41.getGreen()
    << p41.getGreen() << endl;
     cout << p51.getRed() << p51.getGreen()
    << p51.getGreen() << endl;
 
}

void test_Graphics(){
    
}

void test_pics(){
    
}

void test_Circle(){
    
}

void test_Line(){
    
}

void test_Rectangle(){
    
}

void test_Shape(){
    
}

void test_Triangle(){
  
}
