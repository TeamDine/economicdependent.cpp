# economicdependent.cpp
///Implementación de la clase de Dependientes económicos
#include "economicdependent.h"

EconomicDependent::EconomicDependent() { }

EconomicDependent::EconomicDependent(const EconomicDependent& e) : name(e.name), age(e.age) { }

EconomicDependent::EconomicDependent(const Name& n, int& a) : name(n), age(a) { }

Name EconomicDependent::getName() {
    return name;
    }

int EconomicDependent::getAge() {
    return age;
    }

void EconomicDependent::setLast(const Name& n) {
    name = n;
    }

void EconomicDependent::setFirst(const int& a) {
    age = a;
    }

std::string EconomicDependent::toString() {
    std::string result;

    result = "Nombre: ";
    result += name.toString();
    result += "Edad: ";
    result += age;

    return result;
    }
