import os
import shutil

origem = "Downloads"

for arquivo in os.listdir(origem):
    if arquivo.endswith(".pdf"):
        shutil.move(
            os.path.join(origem, arquivo),
            os.path.join(origem, "PDFs", arquivo)
        )