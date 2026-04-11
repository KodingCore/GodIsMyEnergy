# 📘 MainForm

***

***

## I - Identification

* **Facette**: PRLVR
* **Nom**: MainForm
* **Nom du fichier**: `PRLVR_MainForm.md`
* **Rôle**: Modèle de référence complet et prêt à completion pour le fichier MainForm.cs de tous les projets générés.

***

***

```csharp
// FILEID=${AppName}/Src/MainForm.cs
using System;
using System.Windows.Forms;
using ${AppName}.Managers;

namespace ${AppName}
{
    public partial class MainForm : Form
    {
        private readonly LogsManager _logs;

        public MainForm()
        {
            InitializeComponent();
            _logs = new LogsManager();
            _logs.Info("MainForm initialized.");
            Text = "${UsualName}";
        }

        // UI et logique métier à compléter selon les besoins fonctionnels du projet
    }
}
```

*(MainForm)*,
