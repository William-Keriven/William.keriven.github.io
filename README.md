# William.keriven.github.io (debut de d'apprentissage de dev)
// See https://aka.ms/new-console-template for more information
Dictionary<string, int> dico = new Dictionary<string, int>();


/// ecricre sur papier pour préparer au mieux ce qu'on dois coder, plusieurs fois si il le faut 

dico.Add("maths", 8);
dico.Add("ang", 12);
dico.Add("hist", 14);

/// celle ci plus simple et clair pour l'instant 
///on peut faire par une autre ecriture


///dico["maths"] += 8 
///dico["ang"] += 12
///dico["hist"] += 14

foreach (var Ligne in dico)
{
    Console.WriteLine($"la clé est {Ligne.Key} et la valeur est {Ligne.Value} .");
}
/// ecrire avec un un dictionnaire 

if (!dico.ContainsKey("informatique")) 
    /// erreur faite à l'ecriture entre le informatique de if et le maths de la ligne d'en dessous 
{
    dico["maths"] += 8;
}
else
{
    dico["ang"] += 12;

}
foreach (var Ligne in dico)
{
    Console.WriteLine($"la clé est {Ligne.Key} et la valeur est {Ligne.Value} .");
}
