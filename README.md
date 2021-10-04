# Calculadora-de--rea-Java
Codigo de exemplo em Java 
vax.swing.*;
import java.text.DecimalFormat;

public class MedidorTerreno {

    public static void main (String[]args) {

        double largura, comprimento, metroQuadrado, area, precoTotal ;

        largura= Double.parseDouble(JOptionPane.showInputDialog("Digite a largura do Terreno"));
        comprimento= Double.parseDouble(JOptionPane.showInputDialog("Digite o comprimento do Terreno"));
        metroQuadrado= Double.parseDouble(JOptionPane.showInputDialog("Digite o valor do metro quadrado"));

        area = largura * comprimento;
                precoTotal = area * metroQuadrado ;

        DecimalFormat decimal = new DecimalFormat("0.00") ;
        String areaFormatada = decimal.format(area);
        String precoTotalformatada  = decimal.format (precoTotal);

        JOptionPane.showMessageDialog(null,"Area do terreno="+areaFormatada+"\nPreco do terreno="+precoTotalformatada);

  }


}
