# 🎯 Générateur de Why - Trouvez votre raison d'être

Un outil interactif pour découvrir et formuler votre "Why" selon la méthode de Simon Sinek.
**Disponible en 2 versions : personnelle et entreprise (WhyPro).**

## ✨ Nouvelles fonctionnalités

### 🏢 WhyPro - Version Entreprise (NOUVEAU!)
- **Version dédiée aux organisations** : Questions adaptées au contexte B2B
- **Valeurs d'entreprise** : 12 valeurs spécifiques aux organisations
- **Communication corporate** : Styles IA adaptés aux entreprises
- **Branding professionnel** : Couleurs et design corporate
- **Page d'accueil** : Choix entre version personnelle et entreprise

### 🔧 Corrections apportées
- **✅ Encodage PDF corrigé** : Les caractères français (à, é, è, ç, etc.) s'affichent maintenant correctement dans le PDF
- **📄 PDF optimisé une page** : Mise en page compacte en 2 colonnes pour tenir sur une seule page A4
- **🎨 Design amélioré** : Interface plus moderne et responsive

### 🤖 Intégration IA

#### Configuration
1. Dupliquez `.env.example` en `.env`
2. Ajoutez votre clé API OpenAI ou Anthropic
3. L'application détectera automatiquement la configuration

#### Utilisation de l'IA
- Bouton **"🤖 Améliorer avec IA"** disponible sur la page de résultats
- Choix entre OpenAI (GPT-4) et Anthropic (Claude)
- 4 styles d'amélioration disponibles :
  - **Professionnel et impactant** : Pour le monde des affaires
  - **Inspirant et émotionnel** : Pour toucher le cœur
  - **Concis et percutant** : Direct et mémorable
  - **Narratif et engageant** : Raconte une histoire

#### Fonctionnalités IA
- **Génération de 3 versions** alternatives de votre Why
- **Adopter une version** : Remplace votre Why actuel
- **Copier** : Copie une version dans le presse-papiers
- **Sécurité** : Vos clés API ne sont jamais stockées

## 🚀 Utilisation

### Démarrage
1. Ouvrez `index.html` dans votre navigateur
2. Choisissez votre parcours :
   - **Why Personnel** (`whyPerso.html`) : Pour votre raison d'être personnelle
   - **WhyPro** (`whyPro.html`) : Pour la raison d'être de votre entreprise

### Parcours personnel
1. Suivez les 7 étapes guidées
2. Explorez vos motivations et valeurs personnelles
3. Téléchargez votre Why en PDF

### Parcours entreprise (WhyPro)
1. Analysez les origines de votre entreprise
2. Définissez vos valeurs organisationnelles
3. Identifiez votre impact sur le marché
4. Générez le Why de votre organisation

### Avec IA (nouveau)
1. Complétez d'abord le parcours classique
2. Cliquez sur "🤖 Améliorer avec IA"
3. Configurez votre clé API et style préféré
4. Explorez les 3 versions générées
5. Adoptez celle qui vous convient le mieux

### Données de test
- Bouton **"🧪 Charger des données de test"** pour tester rapidement
- Génère un profil d'exemple complet
- Parfait pour découvrir les fonctionnalités

## 🔧 Configuration IA

### Variables d'environnement (.env)
```env
# OpenAI API Key (recommandé)
OPENAI_API_KEY=your_openai_api_key_here

# Anthropic API Key (Claude)
ANTHROPIC_API_KEY=your_anthropic_api_key_here

# Modèle par défaut
AI_MODEL=gpt-4o-mini

# Nombre de versions à générer
AI_VERSIONS_COUNT=3
```

### Obtenir une clé API

#### OpenAI
1. Créez un compte sur [platform.openai.com](https://platform.openai.com)
2. Générez une clé API dans votre dashboard
3. Modèle recommandé : `gpt-4o-mini` (économique et performant)

#### Anthropic
1. Créez un compte sur [console.anthropic.com](https://console.anthropic.com)
2. Générez une clé API
3. Modèle utilisé : `claude-3-sonnet-20240229`

## 📋 Fonctionnalités techniques

- **Framework** : HTML/CSS/JavaScript pur (aucune dépendance)
- **PDF** : jsPDF pour la génération
- **IA** : Support OpenAI et Anthropic APIs
- **Sécurité** : Clés API traitées côté client uniquement
- **Mobile** : Interface responsive
- **Données** : Sauvegarde locale pendant la session

## 🎨 Personnalisation

### Styles disponibles
- Couleurs : Dégradé violet-bleu personnalisable
- Polices : System fonts pour une compatibilité maximale
- Layout : Grid CSS moderne et flexible

### Ajout de nouveaux providers IA
Modifiez la fonction `callAiApi()` pour supporter d'autres APIs comme :
- Google Gemini
- Mistral AI
- APIs locales (Ollama, etc.)

## 📄 Structure des fichiers

```
whyBuilder/
├── index.html          # Page d'accueil pour choisir le parcours
├── whyPerso.html      # Générateur de Why personnel
├── whyPro.html        # Générateur de Why d'entreprise
├── .env.example       # Template de configuration IA
├── .gitignore         # Fichiers à ignorer
└── README.md          # Cette documentation
```

## 🔒 Sécurité et confidentialité

- **Clés API** : Jamais stockées, traitées uniquement côté client
- **Données personnelles** : Restent dans votre navigateur
- **HTTPS requis** : Pour l'utilisation des APIs IA
- **CORS** : Géré par les proxies des APIs

## 🎯 Prochaines améliorations possibles

- [ ] Sauvegarde cloud optionnelle
- [ ] Export en différents formats (Word, PowerPoint)
- [ ] Templates de Why par secteur d'activité
- [ ] Intégration calendrier pour révisions périodiques
- [ ] Version multilingue

---

*Basé sur la méthode "Start With Why" de Simon Sinek*