package proyectorestaurante;


import java.awt.*;
import javax.swing.*;
//import javax.swing.border.Border;

public class Panel extends JFrame {
    JPanel mainPanelUno = new JPanel();
    JPanel mainPanelDos = new JPanel();
    JButton botonIngresar = new JButton("Ingresar");
    JComboBox carta, inventario, registro;
    //JButton botonPagar, botonCancelar;

    public Panel() {
        setLayout(new BorderLayout());
        setSize(600, 400);
        add(mainPanelUno);
        panelUno();
        mainPanelUno.setVisible(false); //llamado
        add(mainPanelDos);
        panelDos();
        mainPanelDos.setVisible(true); 
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

    }

    public void panelUno() {
        
        mainPanelUno.setLayout(new BorderLayout());
        mainPanelUno.setPreferredSize(new Dimension(600, 400));

        JLabel title = new JLabel("Restaurante ¨Las Brisas¨");
        title.setFont(new Font("Yu Gothic UI Semilight", Font.PLAIN, 20));
        mainPanelUno.add(title);
        mainPanelUno.setBackground(Color.decode("#FFD700"));

        botonIngresar.setBackground(Color.LIGHT_GRAY);
        botonIngresar.setBackground(Color.decode("#4653db"));
        mainPanelUno.add(botonIngresar);
        JPanel topPanelUno = new JPanel();
        JPanel bottomPanelUno = new JPanel();

        mainPanelUno.add(topPanelUno, BorderLayout.NORTH);
        mainPanelUno.add(bottomPanelUno, BorderLayout.SOUTH);
        topPanelUno.add(title);
        bottomPanelUno.add(botonIngresar);
        topPanelUno.setPreferredSize(new Dimension(570, 30));
        bottomPanelUno.setPreferredSize(new Dimension(30, 50));

    }
    
    public void panelDos(){
        
        mainPanelDos.setPreferredSize(new Dimension(600, 400));
        mainPanelDos.setLayout(new BorderLayout());
        JPanel topPanel = new JPanel();
        JPanel midPanelUno = new JPanel();
        JPanel midPanelDos = new JPanel();
        JPanel leftPanel = new JPanel();
        JPanel rightPanel = new JPanel();
       
        topPanel.setBackground(Color.decode("#FCD0B4"));
        midPanelUno.setBackground(Color.decode("#F7BFBE"));//#FBAED2
        midPanelDos.setBackground(Color.BLACK);
        leftPanel.setBackground(Color.decode("#FFB6C1"));
        rightPanel.setBackground(Color.decode("#FFD700"));
        
        mainPanelDos.add(topPanel, BorderLayout.NORTH);
        mainPanelDos.add(midPanelUno, BorderLayout.CENTER);
        mainPanelDos.add(midPanelDos, BorderLayout.CENTER);
        mainPanelDos.add(leftPanel, BorderLayout.WEST);
        mainPanelDos.add(rightPanel, BorderLayout.EAST);
        
        leftPanel.setPreferredSize(new Dimension(150, 30));
        midPanelUno.setPreferredSize(new Dimension(220, 30));
        midPanelDos.setPreferredSize(new Dimension(220, 30));
        topPanel.setPreferredSize(new Dimension(30, 30));
        rightPanel.setPreferredSize(new Dimension (200, 30));
        
        //elementos topPanel
        topPanel.setLayout(new FlowLayout(FlowLayout.LEFT));
        //adherir bar menu
        
        
        //Elementos leftPanel
        leftPanel.setLayout(new BoxLayout(leftPanel, BoxLayout.Y_AXIS)); //Y va uno sobre otro
        String[] tipoCarta = { "Entradas y picoteos", "Platos de fondo", "Postres", "Bebestibles"};
        String[] tipoInventario = {"Inventario", "Pila de cosas" };
        String[] tipoRegistro = {"Ventas del Día ", "Venta mensual" };
        //String[] tipoMantenimiento = {"Mantenimiento ", "Pila de cosas" };          
        
        carta = new JComboBox(tipoCarta);
        inventario = new JComboBox(tipoInventario);
        registro = new JComboBox(tipoRegistro);
              
        leftPanel.add(carta);
        leftPanel.add(inventario);
        leftPanel.add(registro);
        
        carta.setEditable(false);
        inventario.setEditable(true);
        registro.setEditable(true);
        
        carta.setSelectedItem("Carta");
        inventario.setSelectedItem("Inventario");
        registro.setSelectedItem("Registro");
        
        //fin elementos leftPanel
        
        //Elementos MenuBar
        JMenuItem archivoItem; 
        JMenuBar menuBar;
        JMenu archivoMenu;
        
        menuBar = new JMenuBar();
        archivoMenu = new JMenu("ARCHIVO");
        archivoItem = new JMenuItem("ARCHIVO");
        
        JMenuItem clientesItem = new JMenuItem("Clientes");
        JMenuItem mantenimientoItem = new JMenuItem("Mantenimiento");
                        
        menuBar.add(archivoMenu);
        archivoMenu.add(clientesItem);
        archivoMenu.add(mantenimientoItem);
        
        menuBar.add(archivoMenu);
        archivoMenu.add(clientesItem);
        archivoMenu.add(mantenimientoItem);
        topPanel.add(menuBar);
        //
        
        //JButton Pagar/Cancelar

        JPanel panelPagar;
        JPanel panelLisPrec;
        JTextArea listaPrecios;
        
        panelPagar= new JPanel();
        panelLisPrec= new JPanel();
        listaPrecios = new JTextArea();
        
        rightPanel.setLayout(new BorderLayout()); //da error
        rightPanel.add(BorderLayout.SOUTH, panelPagar);
        panelPagar.setPreferredSize(new Dimension(200, 70));
        panelPagar.add(new JButton("Pagar")); //inicializa, agrega el estilo de diseño y el boton incluyendo el nombre todo en una linea
        panelPagar.add(new JButton("Cancelar"));
        
        rightPanel.add(BorderLayout.NORTH, panelLisPrec);
        panelLisPrec.setPreferredSize(new Dimension(200, 70));

        //rightPanel.add(PanelListaPrecios, BorderLayout.SOUTH); //da error
        
        //PanelListaPrecios.add(listaPrecios);
        //rightPanel.add(cancelar);
        
        
        //JButtonGroup midPanelUno
        midPanelUno.setLayout(new GridLayout(3, 1));
        ButtonGroup grupoBotones = new ButtonGroup();
        JRadioButton entrada1 = new JRadioButton("Cazuela", false);
        JRadioButton entrada2 = new JRadioButton("Empanada");
        JRadioButton entrada3 = new JRadioButton("Ensalada verde");
        JRadioButton entrada4 = new JRadioButton("Ensalada surtida");
        JRadioButton entrada5 = new JRadioButton("Consomé");
        JRadioButton entrada6 = new JRadioButton("Palta Reina");
        grupoBotones.add(entrada1);
        grupoBotones.add(entrada2);
        grupoBotones.add(entrada3);
        grupoBotones.add(entrada4);
        grupoBotones.add(entrada5);
        grupoBotones.add(entrada6);
        midPanelUno.add(entrada1);
        midPanelUno.add(entrada2);
        midPanelUno.add(entrada3);
        midPanelUno.add(entrada4);
        midPanelUno.add(entrada5);
        midPanelUno.add(entrada6);
        entrada1.setVisible(true);
        midPanelUno.setVisible(true);
       
       //
      
       //JButtonGroup midPanelDos
       midPanelDos.add(new JRadioButton("Risotto"));
       midPanelDos.add(new JRadioButton("Cappellette veg"));
       midPanelDos.add(new JRadioButton("Filete de res salsazul"));
       midPanelDos.add(new JRadioButton("Fetuccini saltado"));
       midPanelDos.add(new JRadioButton("Caldillo de congrio"));
       midPanelDos.add(new JRadioButton("Lasagna Veg"));
       
        midPanelDos.setLayout(new GridLayout(3, 1));
        ButtonGroup grupoBotonesDos = new ButtonGroup();
        JRadioButton fondo1 = new JRadioButton("Risotto", false);
        JRadioButton fondo2 = new JRadioButton("Cappellette veg");
        JRadioButton fondo3 = new JRadioButton("Filete de res salsazul");
        JRadioButton fondo4 = new JRadioButton("Fetuccini saltado");
        JRadioButton fondo5 = new JRadioButton("Caldillo de congrio");
        JRadioButton fondo6 = new JRadioButton("Lasagna Veg");
         
        grupoBotonesDos.add(fondo1);
        grupoBotonesDos.add(fondo2);
        grupoBotonesDos.add(fondo3);
        grupoBotonesDos.add(fondo4);
        grupoBotonesDos.add(fondo5);
        grupoBotonesDos.add(fondo6);
        midPanelDos.add(entrada1);
        midPanelDos.add(entrada2);
        midPanelDos.add(entrada3);
        midPanelDos.add(entrada4);
        midPanelDos.add(entrada5);
        midPanelDos.add(entrada6); 
        
        midPanelDos.setVisible(false);
       //

         

    }

}
