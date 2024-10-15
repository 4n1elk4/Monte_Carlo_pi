## Algorytm napisany na zajęcia akademickie Inteligencja Obliczeniowa
# Algorytm Monte Carlo
Algorytm Monte Carlo używany do oszacowania liczby pi polega na losowaniu 
punktów w kwadracie jednostkowym i sprawdzaniu ile z nich znajduje się wewnątrz 
ćwiartki koła wpisanego w ten kwadrat. Stosunek liczby punktów w tym kole do liczby wszystkich losowych punktów pomnożony przez cztery daje nam szacowaną
wartość liczby pi.

# Opis funkcji
Draw_coordinates(n) - Generuje n losowych współrzędnych (x, y) w przedziale [0, 1]
PI(coordinates) - Przyjmuje zbiór współrzędnych i zwraca estymowaną wartość liczby 
pi na podstawie punktów znajdujących się w kole jednostkowym
Monte_Carlo(n) - Łączy powyższe funkcje
within(coordinates) - Zwraca punkty znajdujące się wewnątrz koła jednostkowego  
outside(coordinates) - Zwraca punkty znajdujące się poza kołem jednostkowym

# Opis wykresów
Pierwsze 4 wykresy pokazują losowo wygenerowane punkty na wykresie. Kolorem czerwonym oznaczone są punkty położone wewnątrz ćwiartki koła i na jej obwodzie, a niebieskim te które leżą po za jej granicami. Widzimy, że wraz ze wzrostem nasza ćwiartka jest wypełniona coraz bardziej.
Wykres nr 5 przedstawia zmianę estymowanej wartości pi wraz ze wzrostem liczby punktów. Możemy zauważyć, że poczatkowo wybierana przez nas ilość generowanych punktów (od 100), dość mocno odstaje od wartości pi. Wraz ze zwiększeniem liczby punktów (aż do 100 000) nasza estymowana wartość coraz mniej odbiega od rzeczywistej wartości.
Wykres nr 6 jest to heatmapa. Ciemny czerwony oraz niebieski kolor wskazują na dużą różnicę między naszą oszacowaną, a rzeczywistą wartością liczby pi. Na tej mapie możemy zaobserwować, że idąc w prawo kolory stają się coraz bardziej blade co wskazuje na to, że nasze wartości szacowane przy użyciu większej ilości punktów są bliższe rzeczywistej wartości pi.
Na wykresie nr 7 widzimy boxploty odpowiednio dla 100, 10000, 100000 wartości. Możemy zaobserwować, że dla 100 "strzałów" nasza wartość wacha się dość mocno, wąsy mają dość dużą szerokość, około 0.8. Dla coraz większej ilości wygenerowanych punktów nasza wartość się znacząco polepsza. Przy 100 000 widzimy, że nawet nasze najbardziej odstające wartości, nie są znacznie oddalone od rzeczywistej wartości pi.
