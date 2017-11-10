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
    Color p(3, 9, 199);
    cout << p << endl;
    Color p21(255, 0, 0);
    Color p31(0, 0, 255);
    Color p41(0, 255, 0);
    Color p51(163, 9, 176);
 
    
    
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

    // test of default constructor
    Graphics p14;
    cout << p14 << endl;
  
    
    // test setPixe()
    Color k = (0, 0, 0)
    Graphics pp(3, 9);
    cout << pp << endl;
    Graphics p22(0, 100, ;
    Graphics p32;
    Graphics p42;
    Graphics p52;
    
    // test of member function: clear()
    \

    
    // you can also do cin >> p1;
    p1.read(cin);
    cout << p1 << endl;
}



void test_pics(){
    // test of writeFile
    
  
    
    // test of the other constructor
    Graphics pp(3, 9);
    cout << pp << endl;
    Graphics p22(0, 100, ;
    Graphics p32;
    Graphics p42;
    Graphics p52;
    
    // test of member function: clear()
    \

    
    // you can also do cin >> p1;
    p1.read(cin);
    cout << p1 << endl;
    
}

void test_Circle(){

    // test of default constructor
    Circle p13;
    cout << p13.getCenter << p13.getRadius << p13.getColor << endl;
   
    
    // test of the other constructor
    Circle ppp();
     cout << ppp.getCenter << ppp.getRadius << ppp.getColor << endl;
    
    // test of member function: setCenter()
    Point a = (5, 0);
    p13.setCenter(a);
    Point b = (0, 0)
    p23.setCenter(b);
    Point c = (100, 100)
    p33.setCenter(c);
    Point d = (5, 0)
    p43.setCenter(d);
    Point e = (67, 35)
    p53.setCenter(e);
    // test of member function: setRadius()
    p13.setRadius(3);
    p23.setRadius(0);
    p33.setRadius(100);
    p43.setRadius(99);
    p53.setRadius(-1);
    // test of member function: setColor()
    Color color1 = (0, 0, 0);
    p13.setColor(color1);
    Color color2 = (255, 0, 0);
    p23.setColor(color2);
    Color color3 = (0, 255, 0);
    p33.setColor(color3);
    Color color4 = (0, 0, 255);
    p43.setColor(color4);
    Color color5 = (255, 255, 255);
    p53.setColor(color4);
    Color color6 = (67, 2, 99);
    
    // test of member functions getX() and getY()
    cout << p13.getCenter() << p13.getRadius() << p13.getColor() << endl;
    cout << p23.getCenter() << p23.getRadius() << p23.getColor() << endl;
    cout << p33.getCenter() << p33.getRadius() << p33.getColor() << endl;
    cout << p43.getCenter() << p43.getRadius() << p43.getColor() << endl;
    cout << p53.getCenter() << p53.getRadius() << p53.getColor() << endl;
   
    
}

void test_Line(){
// test of default constructor
    Line p131;
    cout << getCenter << getRadius << getColor << endl;
   
    
    // test of the other constructor
    Circle ppp( 9);
    cout << ppp << endl;
    
    // test of member function: setCenter()
    Point a = (5, 0);
    p13.setCenter(a);
    Point b = (0, 0)
    p23.setCenter(b);
    Point c = (100, 100)
    p33.setCenter(c);
    Point d = (5, 0)
    p43.setCenter(d);
    Point e = (67, 35)
    p53.setCenter(e);
    // test of member function: setRadius()
    p13.setRadius(3);
    p23.setRadius(0);
    p33.setRadius(100);
    p43.setRadius(99);
    p53.setRadius(-1);
    // test of member function: setColor()
    Color color1 = (0, 0, 0);
    p13.setColor(color1);
    Color color2 = (255, 0, 0);
    p23.setColor(color2);
    Color color3 = (0, 255, 0);
    p33.setColor(color3);
    Color color4 = (0, 0, 255);
    p43.setColor(color4);
    Color color5 = (255, 255, 255);
    p53.setColor(color4);
    Color color6 = (67, 2, 99);
    
    // test of member functions getX() and getY()
    cout << p13.getCenter() << p13.getRadius() << p13.getColor() << endl;
    cout << p23.getCenter() << p23.getRadius() << p23.getColor() << endl;
    cout << p33.getCenter() << p33.getRadius() << p33.getColor() << endl;
    cout << p43.getCenter() << p43.getRadius() << p43.getColor() << endl;
    cout << p53.getCenter() << p53.getRadius() << p53.getColor() << endl;
   
    
}

void test_Rectangle(){
    
}

void test_Shape(){
    
}

void test_Triangle(){
  
  Point v11(20,0);
  Point v21(20,2);
  Point v31(11,15);
  Color c11(160, 20, 103);
  Color c21(157, 130, 250);
  Color c31(43, 170, 230);
  
  Triangle t1(v11, v21, v31, c11, c21, c31);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  Point v41(0,0);
  Point v51(0,2);
  Point v61(1,1);
  Color c41(100, 100, 100);
  Color c51(150, 150, 150);
  Color c61(50, 100, 150);
  
  t1.setVertexOneColor(v41);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  t1.setVertexTwoColor(v51);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  t1.setVertexThreeColor(v61);
  
  
  t1.setVertexOneColor(c41);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  t1.setVertexTwoColor(c51);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  t1.setVertexThreeColor(c61);
  cout << t1.getVertexOne << t1.getVertexTwo << t1.getVertexThree << t1.getVertexOneColor << t1.getVertexTwoColor << t1.getVertexThreeColor;
  
  
  
}




void loadFile(Graphics& drawer)
{   ifstream ins;
    string fileName;
    string remainingChars;
    char shapeLetter;
    //opens file, sets file to fileName
    fileName = openFile(ins);
    drawer.clear();
   //reads in first character, determines shape, calls the shape's functions
   while (ins >> shapeLetter) {
       Triangle createTriangle;
       Rectangle createRectangle;
       Line createLine;
       Circle createCircle;
       
        if (shapeLetter == 'L') {
            ins >> createLine;
            createLine.draw(drawer);
        } else if (shapeLetter == 'C') {
            createCircle.read(ins);
            createCircle.draw(drawer);
        } else if (shapeLetter == 'T') {
            createTriangle.read(ins);
            createTriangle.draw(drawer);
        } else if (shapeLetter == 'R') {
            createRectangle.read(ins);
            createRectangle.draw(drawer);
        } else {
            getline(ins, remainingChars);
            drawer.clear();
            cout << "Error in input file: " << shapeLetter << remainingChars;
        }
   }
    ins.close();
    cout << "[Loaded " << fileName << "]" << endl;
}
