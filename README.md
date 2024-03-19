# Pdfowicz
Autorzy: Michał Soboszek, Paweł Oparczyk, Mirosław Michalik.

Napisana w Kotlinie biblioteka pozwalająca na tworzenie plików pdf.

# addPage( )
Tworzy nową stronę (nowy obiekt klasy Pages)
# addText(page: Pages, text: String, x: Int, y: Int)
Dodaje tekst (obiekt klasy TextBox) na danej stronie na podanych współrzędnych (x, y)
# addImage(page: Pages, imageFilePath: File, x: Int, y: Int)
Dodaje obraz JPEG (obiekt klasy ImageBox) z danej ścieżki na danej stronie na podanych współrzędnych (x, y), wraz z oryginalnymi wymiarami
# addImage(page: Pages, imageFilePath: File, x: Int, y: Int, scale_x: Int, scale_y: Int)
Dodaje obraz JPEG (obiekt klasy ImageBox) z danej ścieżki na danej stronie na podanych współrzędnych (x, y), wraz danymi wymiarami
# addLine(page: Pages, x1: Int, y1: Int, x2: Int, y2: Int)
Dodaje linię (obiekt klasy VectorGraphicsBox) na danej stronie na współrzędnych o początku(x1, y1) oraz końcu (x2, y2) 
# addTriangle(page: Pages, x: Int, y: Int, a: Int)
Dodaje trójkąt (obiekt klasy VectorGraphicsBox) na danej stronie na współrzędnych środka (x, y) i długości boku a
# addSquare(page: Pages, x: Int, y: Int, a: Int)
Dodaje kwadrat (obiekt klasy VectorGraphicsBox) na danej stronie na współrzędnych środka (x, y) i długości boku a
# addCircle(page: Pages, x: Int, y: Int, r: Int )
Dodaje okrąg (obiekt klasy VectorGraphicsBox) na danej stronie na współrzędnych (x, y), i średnicy r
# savePDF( )
Finalizuje zapis pliku PDF oraz “czyści” swoją pamięć (można tworzyć nowy plik)
