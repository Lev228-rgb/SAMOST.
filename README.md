package com.company;

import javax.swing.*;
import java.awt.*;

public class Main {
    public static JFrame gui = new JFrame();
    public static JTextArea text = new JTextArea(6, 50);
    public static JButton ok = new JButton("OK");
    public static JLabel result = new JLabel();

    public static void main(String[] args) {
        ok.addActionListener(e ->
        {
            System.out.println(text.getText());
        });
        gui.setSize(new Dimension(600, 400));
        gui.setLayout(new FlowLayout());
        gui.add(text);
        gui.add(ok);
        gui.add(result);
        gui.setVisible(true);
        gui.setDefaultCloseOperation(WindowConstants.EXIT_ON_CLOSE);

    }
}

