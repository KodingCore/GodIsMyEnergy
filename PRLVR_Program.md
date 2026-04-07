# 📘 Program

***

***

## I - Identification

* **Facette**: PRLVR
* **Sujet**: SCRPT
* **Nom**: Program
* **Nom du fichier**: `PRLVR_Program.md`
* **Rôle**: Point d’entrée C# minimal (prêt à completion).

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
