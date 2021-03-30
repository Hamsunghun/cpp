# cpp#include "car.h""

class Car {
public:
	Car() : name(), cc(0), hp(0) {}
	Car(string name, double cc, double hp) : name(name), cc(cc), hp(hp) {}

	string Getname() {
		return name;
	}
	void Setname(string name_) {
		name = name_;
	}

	double Getkm() {
		return cc;
	}

	void Setkm(double cc_) {
		cc = cc_;
	}

	double Gethp() {
		return hp;
	}

	void Sethp(double hp_) {
		hp = hp_;
	}

private:
	string name;
	double cc;
	double hp;
};
#include <iostream>

using namespace std;
#include "car.cpp""

int main() {
	Car c1{"2020 �ƹݶ�",1598,123};
	Car c2{ "2020 �ҳ�Ÿ",1591,180 };
	Car c3{ "2019 ���̿��� ���̺긮��",1580,105 };
	Car c4{ "2020 ��Ÿ��",2151,202 };

	cout << "�������� = " << c1.Getname() << ", " << "��ⷮ :" << c1.Getkm() << "cc" << ", " << "�ִ���� :" << c1.Gethp() << "hp" << endl;
	cout << "�������� = " << c2.Getname() << ", " << "��ⷮ :" << c2.Getkm() << "cc" << ", " << "�ִ���� :" << c2.Gethp() << "hp" << endl;
	cout << "�������� = " << c3.Getname() << ", " << "��ⷮ :" << c3.Getkm() << "cc" << ", " << "�ִ���� :" << c3.Gethp() << "hp" << endl;
	cout << "�������� = " << c4.Getname() << ", " << "��ⷮ :" << c4.Getkm() << "cc" << ", " << "�ִ���� :" << c4.Gethp() << "hp" << endl;
	
}
