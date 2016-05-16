# herencia
#include <iostream>

using namespace std;

class alumnos
{
public:
    void estudiar()
    {
        cout<<"estudiando...";
    }

};

class primaria : public alumnos
{
    public:
    string materias[6];
    void ingresar(string a)
    {
        for (int i =0;i<6;i++)
            cin>>materias[i];
    }
};
class secundaria : public alumnos
{
    public:
    string materias[8];
    void ingresar(string a)
    {
        for (int i =0;i<8;i++)
            cin>>materias[i];
    }
};



int main()
{
    secundaria A;
    A.estudiar();
    return 0;
}
