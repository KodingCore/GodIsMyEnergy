# 📘 Program

***

***

## I - Identification

* **Facette**: PRLVR
* **Nom**: Program
* **Nom du fichier**: `PRLVR_Program.md`
* **Rôle**: Modèle de référence complet et prêt à completion pour le fichier Program.cs de tous les projets générés.

***

***

```csharp
// FILEID=${AppName}/Src/Program.cs
using System;
using System.Windows.Forms;

namespace ${AppName}
{
    internal static class Program
    {
        [STAThread]
        static void Main()
        {
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new MainForm());
        }
    }
}
```

*(Program)*,
