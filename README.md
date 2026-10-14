# mini-lualatex
A minimal LuaLaTeX tarball, that facilitates LaTeX compilation in a cloud-based Python notebook, such as Colab. The specific task in mind was compiling accessible transcriptions for physics videos (see https://arxiv.org/abs/2608.20733), although in principle this tool should be capable of compiling a large class of LuaLaTeX (Version 1.24.0, TeX Live 2026) files.

CONTENTS:

README.md: This file

LaTeXCloudNotebookCompile.ipynb: Notebook that can be used (with small modifications) to compile .tex files inside of a users Google Drive.

LuaLaTeXCreateLocalInstallandTest.ipynb: Developer notebook for updating the tarball here. The tar.gz which was created in Colab is too big to stick in a github repo, but each version will be attached as a release until we can do something a little better.

USER INSTRUCTIONS:
1. Download LaTeXCloudNotebookCompile.ipynb to your local machine - click the file above, and then click the small download icon in the upper right of the editing window.
2. Go to Google Colab (https://colab.research.google.com/), which should ask you to sign in with your Google Credentials.
3. Upload LaTeXCloudNotebookCompile.ipynb to Colab (Upload Notebook -> Browse for the downloaded file)
4. Open that file in Colab (or it should have opened for you already)
5. Put the .tex file from the AI-assisted transcription process into your top-level Google Drive.
6. In the Colab notebook, change the filename to match what you just uploaded.
7. Run the Notebook with "Run All" at the top of the page.
8. It should run for about a minute, and drop a copy of the compiled pdf in your Google Drive, as well as prompt you to download it.


TO DO:

2. Include Tikz in the pipeline
3. Include PreFigure in the pipeline
