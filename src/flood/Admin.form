import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class Admin extends JFrame {

    public Admin() {
        setTitle("Administrator Panel");
        setSize(600, 400);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null); // center the window

        // Header
        JLabel header = new JLabel("WELCOME ADMINISTRATOR", SwingConstants.CENTER);
        header.setFont(new Font("Arial", Font.BOLD, 20));
        add(header, BorderLayout.NORTH);

        // Panel with buttons
        JPanel buttonPanel = new JPanel(new GridLayout(2, 2, 20, 20));
        buttonPanel.setBorder(BorderFactory.createEmptyBorder(30, 30, 30, 30));

        // Buttons
        JButton orderButton = new JButton("Order");
        JButton campButton = new JButton("Camp");
        JButton officerButton = new JButton("Officer");
        JButton userButton = new JButton("User");

        // Add buttons
        buttonPanel.add(orderButton);
        buttonPanel.add(campButton);
        buttonPanel.add(officerButton);
        buttonPanel.add(userButton);

        add(buttonPanel, BorderLayout.CENTER);

        // Button actions
        orderButton.addActionListener(e -> openWindow("Order Management"));
        campButton.addActionListener(e -> openWindow("Camp Management"));
        officerButton.addActionListener(e -> openWindow("Officer Management"));
        userButton.addActionListener(e -> openWindow("User Management"));

        setVisible(true);
    }

    // Method to open a placeholder window
    private void openWindow(String title) {
        JFrame window = new JFrame(title);
        window.setSize(300, 200);
        window.setLocationRelativeTo(null);
        window.setDefaultCloseOperation(JFrame.DISPOSE_ON_CLOSE);

        JLabel label = new JLabel(title + " Window", SwingConstants.CENTER);
        label.setFont(new Font("Arial", Font.PLAIN, 16));
        window.add(label);

        window.setVisible(true);
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(() -> new Admin());
    }
}
