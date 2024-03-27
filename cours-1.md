# Programation générative

Pour créer un template de fonction :

```cpp
template<typename Type>
Type minimum(Type a, Type b)
{
	return a<b ? a : b;
}
```

Et pour l'appeler :

```cpp
auto x = minimum(4, 5);
```

Erreur de déduction si on envoit un double et un int par exemple, la fonction déduit à la fin qu'il y a une erreur.

Etape de substitution : identifier les types et mettre en place les valeurs.

Si le compilateur échoue dans la compilation du template, il continue et va chercher une fonction ailleurs.

Si il ne trouve pas d'autre fonctions après l'erreur du template : "No matching functions". [Echec de substitution]

Un echec de substituion n'est **PAS** une erreur.
