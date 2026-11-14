<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jasper Chavoso - Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="logo">JASPER<span>.</span></div>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#education">Education</a>
            <a href="#skills">Skills</a>
            <a href="#java">Java Code</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="home" class="home">
        <div class="home-text">
            <h3>Hi, I am</h3>
            <h1>Jasper Chavoso</h1>
            <h2>BSIT 1-A | OLSHCO Guimba</h2>
            <p>Applying for Junior Programmer position at JPCS Inc. I am a first-year BS Information Technology student passionate about programming and web development.</p>
            <div class="buttons">
                <a href="#java" class="btn-dark">View My Project</a>
                <a href="#contact" class="btn-light">Contact Me</a>
            </div>
        </div>
        <div class="home-img">
            <img src="jasper.jpg" alt="Jasper Chavoso">
        </div>
    </section>

    <section id="about">
        <h2 class="title">Personal Information</h2>
        <div class="box">
            <p><b>Name:</b> Jasper Chavoso</p>
            <p><b>Course:</b> BS Information Technology - 1A</p>
            <p><b>School:</b> Our Lady of the Sacred Heart College of Guimba, Inc.</p>
            <p><b>Address:</b> Guimba, Nueva Ecija, Philippines</p>
            <p><b>Email:</b> jasperchavoso@gmail.com</p>
            <p><b>About Me:</b> Ako si Jasper, 19 years old. Mahilig ako sa computer games at gusto ko matuto gumawa ng sarili kong games at websites. Kaya ko nag BSIT para maging programmer balang araw. Ginawa ko itong portfolio para sa CC101 & CC102 Finals.</p>
        </div>
    </section>

    <section id="education">
        <h2 class="title">Educational Background</h2>
        <div class="grid">
            <div class="card">
                <h3>College</h3>
                <p>BS Information Technology</p>
                <p>Our Lady of the Sacred Heart College of Guimba</p>
                <span>2025 - Present</span>
            </div>
            <div class="card">
                <h3>Senior High School</h3>
                <p>[Ilagay mo SHS mo dito]</p>
                <p>Guimba, Nueva Ecija</p>
                <span>2023 - 2025</span>
            </div>
            <div class="card">
                <h3>Junior High School</h3>
                <p>[Ilagay mo JHS mo dito]</p>
                <span>2019 - 2023</span>
            </div>
        </div>
    </section>

    <section id="skills">
        <h2 class="title">Skills</h2>
        <div class="skills-box">
            <div class="skill">
                <h4>Technical Skills</h4>
                <p>HTML, CSS, Basic Java, MS Word, Excel, PowerPoint, Video Editing, Computer Troubleshooting</p>
            </div>
            <div class="skill">
                <h4>Programming Knowledge</h4>
                <p>Understanding of basic programming logic, loops, conditionals, and console-based application in Java.</p>
            </div>
            <div class="skill">
                <h4>Other Skills</h4>
                <p>Time Management, Willing to Learn, Teamwork, Communication</p>
            </div>
        </div>
    </section>

    <section id="java">
        <h2 class="title">Java Code - CC102 Final PeTa</h2>
        <p class="subtitle">Console-Based Game - Final Performance Task in CC102</p>
        <div class="code-box">
            <h3>Number Guessing Game - by Jasper Chavoso BSIT 1-A</h3>
            <p>This is my console-based game made in Java for CC102. The player needs to guess the secret number from 1 to 100.</p>
            <pre><code>import java.util.Scanner;
import java.util.Random;

public class NumberGuessingGame {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Random rand = new Random();

        System.out.println("=================================");
        System.out.println(" NUMBER GUESSING GAME ");
        System.out.println(" Gawa ni: Jasper Chavoso - BSIT 1-A ");
        System.out.println(" CC102 Final PeTa ");
        System.out.println("=================================");

        System.out.print("Enter your name: ");
        String name = sc.nextLine();

        int secretNumber = rand.nextInt(100) + 1;
        int guess = 0;
        int attempts = 0;

        System.out.println("\nHello " + name + "! I have a number from 1 to 100.");
        System.out.println("Can you guess it?");

        while (guess != secretNumber) {
            System.out.print("\nYour guess: ");
            guess = sc.nextInt();
            attempts++;

            if (guess < secretNumber) {
                System.out.println("Too low! Try higher.");
            } else if (guess > secretNumber) {
                System.out.println("Too high! Try lower.");
            } else {
                System.out.println("\nCongratulations " + name + "!");
                System.out.println("You guessed it in " + attempts + " tries!");
                System.out.println("The secret number is " + secretNumber);
            }
        }
        System.out.println("Thank you for playing!");
        sc.close();
    }
}</code></pre>
            <p class="explain"><b>Explanation:</b> Gumamit ako ng Random para pumili ng secret number, Scanner para sa input ng user, while loop para paulit-ulit hanggang mahulaan, at if-else para sabihin kung too high or too low.</p>
        </div>
    </section>

    <section id="contact">
        <h2 class="title">Contact Information</h2>
        <div class="contact-box">
            <p>Email: jasperchavoso@gmail.com</p>
            <p>Facebook: Jasper Chavoso</p>
            <p>Location: Guimba, Nueva Ecija</p>
            <p>GitHub: github.com/jasperchavoso13</p>
            <br>
            <p>This portfolio is for CC101 & CC102 FINALS - OLSHCO</p>
            <p>BUILD DREAMS. CODE FUTURES | Ex Fide, Ad Futurum</p>
        </div>
    </section>

    <footer>
        <p>© 2026 Jasper Chavoso | BSIT 1-A | OLSHCO Guimba | Designed inspired by Jemouldin Portfolio</p>
    </footer>

</body>
</html>
