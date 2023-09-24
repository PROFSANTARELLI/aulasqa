# aulasqa
Aulas de QA
import unittest

class Calculadora:
    def adicionar(self, a, b):
        return a + b

    def subtrair(self, a, b):
        return a - b

# Definir uma classe de teste para a Calculadora
class TestCalculadora(unittest.TestCase):

    def setUp(self):
        # Configurações iniciais, se necessário
        pass

    def tearDown(self):
        # Limpeza após os testes, se necessário
        pass

    def test_adicionar(self):
        calc = Calculadora()
        resultado = calc.adicionar(2, 3)
        self.assertEqual(resultado, 5)  # Verificar se a adição está correta

    def test_subtrair(self):
        calc = Calculadora()
        resultado = calc.subtrair(5, 3)
        self.assertEqual(resultado, 2)  # Verificar se a subtração está correta

if __name__ == '__main__':
    unittest.main()
