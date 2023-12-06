# Tela-de-Cadastro-

package anaecaua;

import java.awt.Color;
import java.awt.Font;

import javax.swing.ButtonGroup;
import javax.swing.ImageIcon;
import javax.swing.JButton;
import javax.swing.JCheckBox;
import javax.swing.JComboBox;
import javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.JRadioButton;
import javax.swing.JTextField;
@SuppressWarnings("serial")


public class anaecaua extends JFrame {
	JButton bt1, bt2, bt3;
	ImageIcon img ;
	JLabel lb1,lb2, lb3, lb4,lb5, lb6, lb7,lb8;
	JTextField tx1, txt2,txt3,txt4, txt5;


	public anaecaua() {
		//imagem
		setSize(900,900);
		img=new ImageIcon(getClass().getResource("ana.jpg"));
		
		//nome da tela
		setTitle("Cadastro");
		setResizable(false);
		setLocationRelativeTo(null);
		
		//botoes
		
		JButton bt1=new JButton("cancelar");
		bt1.setBounds(130, 450, 90,30);
		bt1.setBackground(Color.white);
		add(bt1);
		
		JButton bt2=new JButton("ok");
		bt2.setBounds(290, 450, 70,30);
		bt2.setBackground (Color.white);
		add(bt2);
		
		JButton bt3=new JButton("editar");
		bt3.setBounds(430, 450, 70,30);
		bt3.setBackground (Color.white);
		add(bt3);
		//botoes
		
		// escrita de texto
		JTextField tx1= new JTextField();
	   tx1.setBounds(160, 120, 100, 30);
	   add(tx1);
	   
	   JTextField txt2= new JTextField();
	   txt2.setBounds(160, 160, 100, 30);
	   add(txt2);
	   
	   JTextField txt3= new JTextField();
	   txt3.setBounds(160, 200, 100, 30);
	   add(txt3);
	   
	   JTextField txt4= new JTextField();
	   txt4.setBounds(160, 240, 100, 30);
	   add(txt4);
	   
	   JTextField txt5= new JTextField();
	   txt5.setBounds(160, 280, 100, 30);
	   add(txt5);
	   
	   //texto
	   
		JLabel lb2 = new JLabel("Nome:");
		lb2.setBounds(50, 100, 100,70);
		lb2.setFont(new Font("arial",5,25));
		lb2.setForeground(Color.white);
		add(lb2);
	
		JLabel lb3 = new JLabel("Idade:");
		lb3.setBounds(50, 140, 100,70);
		lb3.setFont(new Font("arial",5,25));
		lb3.setForeground(Color.white);
		add(lb3);
		
		JLabel lb4 = new JLabel("telefone:");
		lb4.setBounds(50, 180, 110,70);
		lb4.setFont(new Font("arial",5,25));
		lb4.setForeground(Color.white);
		add(lb4);
		
		JLabel lb5 = new JLabel("cidade:");
		lb5.setBounds(50, 220, 300,70);
		lb5.setFont(new Font("arial",6,25));
		lb5.setForeground(Color.white);
		add(lb5);
		
		JLabel lb6 = new JLabel("login:");
		lb6.setBounds(50, 260, 100,70);
		lb6.setFont(new Font("arial",5,25));
		lb6.setForeground(Color.white);
		add(lb6);
		
		JLabel lb7 = new JLabel("Genero:");
		lb7.setBounds(350, 100, 100,70);
		lb6.setFont(new Font("arial",5,5));
		lb7.setForeground(Color.white);
		add(lb7);
		
	    JLabel lb8 = new JLabel("CADASTRO");
		lb8.setBounds(50, 60, 100,70);
		lb8.setFont(new Font("arial",1,17));
		lb8.setForeground(Color.white);
		add(lb8);
		
		JLabel lb9 = new JLabel("termos:");
		lb9.setBounds(500, 100, 100,70);
		lb9.setFont(new Font("arial",5,25));
		lb9.setForeground(Color.white);
		add(lb9);
		
		JLabel lb10 = new JLabel("etnias:");
		lb10.setBounds(670, 100, 100,70);
		lb10.setFont(new Font("arial",5,25));
		lb10.setForeground(Color.white);
		add(lb10);
		
		//imagem de fundo
		lb1=new JLabel(img);
		lb1.setBounds(0, 0, 900, 900);
		add(lb1);
		
		ButtonGroup grupo1= new ButtonGroup ();
		
		
		JRadioButton rd1= new JRadioButton("masculino");
		JRadioButton rd2= new JRadioButton("feminino");
		JRadioButton rd3= new JRadioButton("não binário");
		
		rd1.setBounds(350,160,90,30);
		rd2.setBounds(350,200,80,30);
		rd3.setBounds(350,240,100,30);
		
		
		setLayout(null);
		
		grupo1.add(rd1);
		grupo1.add(rd2);
		grupo1.add(rd3);
		
		
		add(rd1);
		add(rd2);
		add(rd3);
		
		//opções//
	String s1[] = {"Negro", "Branco", "Pardo"};
		
		JComboBox<String> c1 = new JComboBox<String>(s1);
		c1.setBounds(670,150, 128, 50);
		add(c1);
		
		 JCheckBox v1 = new  JCheckBox("sim");
		 v1.setBounds(500, 150, 128, 50);
		 add(v1);
		 
		 JCheckBox v2 = new  JCheckBox("não");
		 v2.setBounds(500, 210, 128, 50);
		 add(v2);
		
		lb7 = new JLabel(img);
		lb7.setBounds(0, 0, 500, 500);
		add(lb7);
	    
		
	}
	
	public static void main(String[] args) {
		anaecaua ca= new anaecaua();
		ca.setVisible(true);
		
	}
}
