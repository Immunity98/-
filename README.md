#include "stdafx.h"
#include <iostream>
#include <conio.h>
#include <math.h>
using namespace std;
void main() {
	float S, Mc, R, p;
	int i = 20, Ax, Ay, Bx = i, By = i - 1, a, b, c, Cx = (-i), Cy = i + 1;
	Ax = Ay = 0;
	b = sqrt(pow((Ax - Bx), 2) + pow((Ay - By), 2));
	c = sqrt(pow((Ax - Cx), 2) + pow((Ay - Cy), 2));
	a = sqrt(pow((Cx - Bx), 2) + pow((Cy - By), 2));
	Mc = 1 / 2 * sqrt(2 * pow(a, 2) * 2 * pow(b, 2) - pow(c, 2)); //mc = 1/2•?(2•a? + 2•b? - c?).
	p = (a + b + c) / 2;
	S = sqrt(p * (p - a) * (p - b) * (p - c));
	R = (a * b * c) / (4 * S);
	cout << "Mc = " << Mc << "\n";
	cout << "S = " << S << "\n";
	system (" pause ");
}
