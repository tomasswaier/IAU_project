# IAU_project

Pridal som sekciu 1.3, dodal pár variables do 1.1 D a Spravil 1.1 E. Určite by sa s tým dalo ešte troška pohrať aby to bolo krajšie a menej zbytočnosí ale do odovzdania je to OK si myslím.



todo : pridanie komentarov (Sú tam zatiaľ odo mňa veľmi jednoducho resp. vôbec, v kľude mi napíš či tam chceš v nedeľu nejaké lepšie pridať spolu, alebo či mám nejaké k mojej časti ešte hodiť ja) . 1.1.E : niečo som tam vložil, potom sa na to pozri a rozhodni sa či tam niečo chceš pridávať ešte podľa 1.1 A & B


mohol by si pridať nejako lepšie sformovaný output na tie hypotézy ako bolo v hw kde sme mali niečo ako :
if p>0.05:
    print("meowmeowmeoowo")
else :
    print ("meow moew meow NOT")


do budúcna to asi skús robiť trochu viac abstraktné. Nič si neurobil zle len si si mohol veľmi uľahčiť prácu napr takto

def display_boxplot(y,title,):
    plt.figure(figsize=(10, 6))
    sns.boxplot(x='mwra', y=y, data=df_connections)
    plt.title(title, fontsize=16)
    plt.xlabel('mwra', fontsize=12)
    plt.ylabel(y, fontsize=12)
    plt.show()
    group1 = df_connections[df_connections['mwra'] == 0][y]
    group2 = df_connections[df_connections['mwra'] == 1][y]
    t_stat, p_value = stats.ttest_ind(group1, group2)
    print(f"T-statistic: {t_stat}, P-value: {p_value}")
display_boxplot('c.dogalize','Box Plot of c.dogalize vs mwra')

a toto by si iba zavolal X krát na každú premennú čo potrebuješ porovnať s mwra namiesto manuálneho písania Y variables X krát
