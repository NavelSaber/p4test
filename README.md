# p4test
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
