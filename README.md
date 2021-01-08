# GUI2
ex2
import java.awt.Color;

import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JPanel;

public class GUI3 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		JFrame.setDefaultLookAndFeelDecorated(true);//çerceve şekli
		JFrame frame=new JFrame("Renklerle Çalışıyoruz");
		
		JPanel GUI=new JPanel();
		GUI.setLayout(null);
		
		JPanel yazılar=new JPanel();
		yazılar.setLayout(null);
		yazılar.setLocation(10,0);
		yazılar.setSize(150,30);
		GUI.add(yazılar);
		
		
		JLabel kırmızı=new JLabel("kırmızı");
		kırmızı.setLocation(0,0);
		kırmızı.setSize(50,30);
		kırmızı.setHorizontalAlignment(0);// 0 merkez 2 sola 4 sağa yaslama
		yazılar.add(kırmızı);		
		
		JLabel beyaz=new JLabel("beyaz");
		beyaz.setLocation(100,0);
		beyaz.setSize(50,30);
		beyaz.setHorizontalAlignment(0);
		yazılar.add(beyaz);
		
		
		JPanel renkler=new JPanel();
		renkler.setLayout(null);
		renkler.setLocation(10,40);
		renkler.setSize(150,50);
		GUI.add(renkler);
		
		JPanel kırmızıkutu=new JPanel();
		kırmızıkutu.setBackground(Color.red);
		kırmızıkutu.setLocation(50,50);
		kırmızıkutu.setSize(50,50);
		renkler.add(kırmızıkutu);
		
		JPanel beyazkutu=new JPanel();
		beyazkutu.setBackground(Color.white);
		beyazkutu.setLocation(100,0);
		beyazkutu.setSize(50,50);
		renkler.add(beyazkutu);
		
		frame.setSize(190,150);
		frame.setContentPane(GUI);
		frame.setResizable(false);//çerceve boyutu sabit
		frame.setVisible(true);
		
		
		
	}

}
