Cover Letter Template
A professional LaTeX-based cover letter template system designed for creating personalized French cover letters with modular content management and professional formatting.  
Features

Professional Formatting: Uses the moderncv document class with classic styling  
French Localization: Full French language support with proper typography and date formatting  
Modular Architecture: Separate template files for different sections of the cover letter  
Easy Customization: Simple placeholder-based content substitution  
PDF Generation: Automated compilation to professional PDF documents

Attribution
This template was originally based on the Harvard Extension School's resume and cover letter guide: 2024 HES Resume and Letter Guide. It has been adapted and customized for French professional correspondence using the moderncv LaTeX document class.
Requirements

LaTeX distribution (TeX Live, MiKTeX, or MacTeX)  
Required packages:  
moderncv  
babel (French)  
noto fonts  
geometry



Project Structure
├── main.tex                  # Main document controller
├── main.pdf                  # Generated cover letter (output)
└── sections/
    ├── RightHeader.tex       # Personal contact information
    ├── OpeningParagraph.tex  # Application introduction
    ├── MiddleParagraph.tex   # Experience alignment content
    └── ClosingParagraph.tex  # Professional closing

Quick Start

Clone the repository:  
git clone https://github.com/fedei10/cover-letter-template.git  
cd cover-letter-template  


Customize your personal information in sections/RightHeader.tex:  
\name{Your First Name}{Your Last Name}  
\phone[mobile]{+33 X XX XX XX XX}  
\email{your.email@example.com}  
\address{Your Address}{City, Postal Code}


Update recipient information in main.tex (lines 33-37):  
\recipient{Contact Name}{%
Contact Title\\
Company Name\\
Address\\
Postal Code, City}


Customize content sections:  

Edit sections/OpeningParagraph.tex for your introduction  
Modify sections/MiddleParagraph.tex to align your experience with the role  
Update sections/ClosingParagraph.tex for your closing statement


Compile the document:  
pdflatex main.tex



Configuration

Document Class: moderncv with 11pt font, A4 paper, roman style  
Style Theme: Classic professional appearance  
Color Scheme: Green corporate palette  
Page Layout: 75% scale for optimized margins  
Typography: Noto font family for professional appearance

Template Sections

Personal Header (sections/RightHeader.tex): Contains your contact information using moderncv commands for consistent formatting.  
Content Structure: The cover letter follows a three-part narrative structure:  
Opening: Job application introduction and interest statement  
Middle: Experience-to-role alignment and qualifications  
Closing: Professional closing and call-to-action



Compilation Output
The system generates:  

main.pdf - Final formatted cover letter  
main.synctex.gz - Editor synchronization data for LaTeX IDEs

French Language Features

Proper French hyphenation and typography via babel  
UTF-8 encoding for accented characters  
Automatic French date formatting  
Professional French business letter conventions

Customization Tips

Modify the color scheme by changing \moderncvcolor{green} to other available colors  
Adjust page margins by modifying the geometry package scale parameter  
Add additional sections by creating new .tex files in the sections/ directory  
Customize the closing formula and enclosures as needed for your application

License
This template is provided as-is for personal and professional use.  
Notes
This README provides a comprehensive overview of the LaTeX cover letter template system. The template uses a modular architecture where the main controller orchestrates various content sections, making it easy for users to customize their cover letters while maintaining professional formatting standards. The French localization features and moderncv styling ensure the output meets professional French business correspondence standards.  
Wiki pages you might want to explore:  

Overview (fedei10/cover-letter)

