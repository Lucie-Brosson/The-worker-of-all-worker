import { useState } from "react";

const DEFAULT_SITES = [
  { id: 1, name: "Welcome to the Jungle", url: "https://www.welcometothejungle.com", active: true },
  { id: 2, name: "APEC", url: "https://www.apec.fr", active: true },
  { id: 3, name: "Job That Makes Sense", url: "https://jobs.makesense.org", active: true },
  { id: 4, name: "Choisir le Service Public", url: "https://choisirleservicepublic.gouv.fr", active: true },
];

const DEFAULT_KEYWORDS = ["Chef de projet", "Conceptrice pédagogique", "Médiation numérique", "Coordinatrice pédagogique", "Ingénierie pédagogique"];

const MOCK_OFFERS = [
  { id: 1, title: "Concepteur·rice pédagogique", company: "Docaposte", location: "Paris (75)", date: "Aujourd'hui", site: "Welcome to the Jungle", url: "#", tag: "Ingénierie pédagogique" },
  { id: 2, title: "Chef·fe de projet digital", company: "Galileo Global Education", location: "Paris (75)", date: "Aujourd'hui", site: "APEC", url: "#", tag: "Chef de projet" },
  { id: 3, title: "Chargé·e de médiation numérique", company: "Paris Musées", location: "Paris (75)", date: "Hier", site: "Choisir le Service Public", url: "#", tag: "Médiation numérique" },
  { id: 4, title: "Coordinateur·rice pédagogique", company: "Groupe ESRA", location: "Paris (75)", date: "Aujourd'hui", site: "Job That Makes Sense", url: "#", tag: "Coordinatrice pédagogique" },
  { id: 5, title: "Chef·fe de projet e-learning", company: "Pix", location: "Paris (75)", date: "Hier", site: "Welcome to the Jungle", url: "#", tag: "Chef de projet" },
];

const SITE_COLORS = {
  "Welcome to the Jungle": { bg: "#E1F5EE", text: "#0F6E56", border: "#5DCAA5" },
  "APEC": { bg: "#E6F1FB", text: "#185FA5", border: "#85B7EB" },
  "Job That Makes Sense": { bg: "#FAEEDA", text: "#854F0B", border: "#EF9F27" },
  "Choisir le Service Public": { bg: "#EEEDFE", text: "#3C3489", border: "#AFA9EC" },
};

export default function App() {
  const [tab, setTab] = useState("config");
  const [sites, setSites] = useState(DEFAULT_SITES);
  const [keywords, setKeywords] = useState(DEFAULT_KEYWORDS);
  const [location, setLocation] = useState("Paris / Île-de-France");
  const [email, setEmail] = useState("");
  const [hour, setHour] = useState("08:00");
  const [newSiteName, setNewSiteName] = useState("");
  const [newSiteUrl, setNewSiteUrl] = useState("");
  const [newKeyword, setNewKeyword] = useState("");
  const [sent, setSent] = useState(false);
  const [activeKeywordFilter, setActiveKeywordFilter] = useState(null);

  const addSite = () => {
    if (!newSiteName.trim()) return;
    setSites([...sites, { id: Date.now(), name: newSiteName.trim(), url: newSiteUrl.trim(), active: true }]);
    setNewSiteName(""); setNewSiteUrl("");
  };

  const removeSite = (id) => setSites(sites.filter(s => s.id !== id));
  const toggleSite = (id) => setSites(sites.map(s => s.id === id ? { ...s, active: !s.active } : s));

  const addKeyword = () => {
    if (!newKeyword.trim() || keywords.includes(newKeyword.trim())) return;
    setKeywords([...keywords, newKeyword.trim()]);
    setNewKeyword("");
  };

  const removeKeyword = (k) => setKeywords(keywords.filter(kw => kw !== k));

  const filteredOffers = activeKeywordFilter
    ? MOCK_OFFERS.filter(o => o.tag === activeKeywordFilter)
    : MOCK_OFFERS;

  const handleSend = () => {
    setSent(true);
    setTimeout(() => setSent(false), 3000);
  };

  const tabStyle = (t) => ({
    padding: "8px 20px",
    borderRadius: "var(--border-radius-md)",
    border: "none",
    cursor: "pointer",
    fontSize: "14px",
    fontWeight: tab === t ? "500" : "400",
    background: tab === t ? "var(--color-background-primary)" : "transparent",
    color: tab === t ? "var(--color-text-primary)" : "var(--color-text-secondary)",
    boxShadow: tab === t ? "0 0 0 0.5px var(--color-border-secondary)" : "none",
  });

  return (
    <div style={{ padding: "1.5rem 0", fontFamily: "var(--font-sans)" }}>
      <h2 className="sr-only">Bot de veille emploi — configuration newsletter</h2>

      <div style={{ marginBottom: "1.5rem" }}>
        <p style={{ fontSize: "13px", color: "var(--color-text-secondary)", margin: "0 0 1rem" }}>
          Configure tes sources, mots-clés et préférences d'envoi ci-dessous.
        </p>
        <div style={{ display: "flex", gap: "6px", background: "var(--color-background-secondary)", padding: "4px", borderRadius: "var(--border-radius-md)", width: "fit-content" }}>
          <button style={tabStyle("config")} onClick={() => setTab("config")}>Configuration</button>
          <button style={tabStyle("preview")} onClick={() => setTab("preview")}>Aperçu des offres</button>
          <button style={tabStyle("script")} onClick={() => setTab("script")}>Script Python</button>
        </div>
      </div>

      {tab === "config" && (
        <div style={{ display: "flex", flexDirection: "column", gap: "1.5rem" }}>

          {/* Sites */}
          <div style={{ background: "var(--color-background-primary)", border: "0.5px solid var(--color-border-tertiary)", borderRadius: "var(--border-radius-lg)", padding: "1.25rem" }}>
            <p style={{ margin: "0 0 1rem", fontWeight: "500", fontSize: "15px" }}>Sites surveillés</p>
            <div style={{ display: "flex", flexDirection: "column", gap: "8px", marginBottom: "1rem" }}>
              {sites.map(s => (
                <div key={s.id} style={{ display: "flex", alignItems: "center", gap: "10px", padding: "8px 12px", background: "var(--color-background-secondary)", borderRadius: "var(--border-radius-md)" }}>
                  <input type="checkbox" checked={s.active} onChange={() => toggleSite(s.id)} style={{ accentColor: "#1D9E75", width: "16px", height: "16px", cursor: "pointer" }} />
                  <span style={{ flex: 1, fontSize: "14px", color: s.active ? "var(--color-text-primary)" : "var(--color-text-tertiary)", textDecoration: s.active ? "none" : "line-through" }}>{s.name}</span>
                  {s.url && <span style={{ fontSize: "12px", color: "var(--color-text-tertiary)" }}>{s.url.replace("https://", "")}</span>}
                  <button onClick={() => removeSite(s.id)} style={{ background: "none", border: "none", cursor: "pointer", color: "var(--color-text-tertiary)", padding: "2px", lineHeight: 1 }}>
                    <i className="ti ti-x" style={{ fontSize: "16px" }} aria-label="Supprimer"></i>
                  </button>
                </div>
              ))}
            </div>
            <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr auto", gap: "8px" }}>
              <input value={newSiteName} onChange={e => setNewSiteName(e.target.value)} placeholder="Nom du site" style={{ fontSize: "13px" }} onKeyDown={e => e.key === "Enter" && addSite()} />
              <input value={newSiteUrl} onChange={e => setNewSiteUrl(e.target.value)} placeholder="URL (optionnel)" style={{ fontSize: "13px" }} onKeyDown={e => e.key === "Enter" && addSite()} />
              <button onClick={addSite} style={{ padding: "0 14px", fontSize: "13px" }}>
                <i className="ti ti-plus" aria-hidden="true"></i> Ajouter
              </button>
            </div>
          </div>

          {/* Mots-clés */}
          <div style={{ background: "var(--color-background-primary)", border: "0.5px solid var(--color-border-tertiary)", borderRadius: "var(--border-radius-lg)", padding: "1.25rem" }}>
            <p style={{ margin: "0 0 1rem", fontWeight: "500", fontSize: "15px" }}>Mots-clés de recherche</p>
            <div style={{ display: "flex", flexWrap: "wrap", gap: "8px", marginBottom: "1rem" }}>
              {keywords.map(k => (
                <span key={k} style={{ display: "inline-flex", alignItems: "center", gap: "6px", background: "#EEEDFE", color: "#3C3489", border: "0.5px solid #AFA9EC", borderRadius: "999px", padding: "4px 12px", fontSize: "13px" }}>
                  {k}
                  <button onClick={() => removeKeyword(k)} style={{ background: "none", border: "none", cursor: "pointer", color: "#534AB7", padding: 0, lineHeight: 1 }}>
                    <i className="ti ti-x" style={{ fontSize: "13px" }} aria-label="Supprimer"></i>
                  </button>
                </span>
              ))}
            </div>
            <div style={{ display: "flex", gap: "8px" }}>
              <input value={newKeyword} onChange={e => setNewKeyword(e.target.value)} placeholder="Ajouter un mot-clé" style={{ flex: 1, fontSize: "13px" }} onKeyDown={e => e.key === "Enter" && addKeyword()} />
              <button onClick={addKeyword} style={{ padding: "0 14px", fontSize: "13px" }}>
                <i className="ti ti-plus" aria-hidden="true"></i> Ajouter
              </button>
            </div>
          </div>

          {/* Email + localisation + heure */}
          <div style={{ background: "var(--color-background-primary)", border: "0.5px solid var(--color-border-tertiary)", borderRadius: "var(--border-radius-lg)", padding: "1.25rem" }}>
            <p style={{ margin: "0 0 1rem", fontWeight: "500", fontSize: "15px" }}>Envoi et filtres</p>
            <div style={{ display: "flex", flexDirection: "column", gap: "12px" }}>
              <div style={{ display: "grid", gridTemplateColumns: "140px 1fr", alignItems: "center", gap: "12px" }}>
                <label style={{ fontSize: "13px", color: "var(--color-text-secondary)" }}>E-mail de réception</label>
                <input value={email} onChange={e => setEmail(e.target.value)} placeholder="ton@email.fr" type="email" style={{ fontSize: "13px" }} />
              </div>
              <div style={{ display: "grid", gridTemplateColumns: "140px 1fr", alignItems: "center", gap: "12px" }}>
                <label style={{ fontSize: "13px", color: "var(--color-text-secondary)" }}>Localisation</label>
                <input value={location} onChange={e => setLocation(e.target.value)} style={{ fontSize: "13px" }} />
              </div>
              <div style={{ display: "grid", gridTemplateColumns: "140px 1fr", alignItems: "center", gap: "12px" }}>
                <label style={{ fontSize: "13px", color: "var(--color-text-secondary)" }}>Heure d'envoi</label>
                <input type="time" value={hour} onChange={e => setHour(e.target.value)} style={{ fontSize: "13px", width: "120px" }} />
              </div>
            </div>
          </div>

          <button onClick={handleSend} style={{ alignSelf: "flex-start", padding: "10px 24px", fontSize: "14px", fontWeight: "500" }}>
            {sent ? <><i className="ti ti-check" aria-hidden="true"></i> Newsletter envoyée !</> : <><i className="ti ti-mail" aria-hidden="true"></i> Envoyer la newsletter maintenant</>}
          </button>
        </div>
      )}

      {tab === "preview" && (
        <div>
          <div style={{ display: "flex", gap: "8px", flexWrap: "wrap", marginBottom: "1rem", alignItems: "center" }}>
            <span style={{ fontSize: "13px", color: "var(--color-text-secondary)" }}>Filtrer :</span>
            <button onClick={() => setActiveKeywordFilter(null)} style={{ fontSize: "12px", padding: "4px 12px", borderRadius: "999px", border: "0.5px solid var(--color-border-secondary)", background: !activeKeywordFilter ? "var(--color-background-secondary)" : "transparent", cursor: "pointer", color: "var(--color-text-primary)" }}>Tout</button>
            {keywords.map(k => (
              <button key={k} onClick={() => setActiveKeywordFilter(k === activeKeywordFilter ? null : k)} style={{ fontSize: "12px", padding: "4px 12px", borderRadius: "999px", border: "0.5px solid var(--color-border-secondary)", background: activeKeywordFilter === k ? "#EEEDFE" : "transparent", color: activeKeywordFilter === k ? "#3C3489" : "var(--color-text-primary)", cursor: "pointer" }}>{k}</button>
            ))}
          </div>
          <div style={{ display: "flex", flexDirection: "column", gap: "10px" }}>
            {filteredOffers.map(o => {
              const c = SITE_COLORS[o.site] || { bg: "#F1EFE8", text: "#5F5E5A", border: "#B4B2A9" };
              return (
                <div key={o.id} style={{ background: "var(--color-background-primary)", border: "0.5px solid var(--color-border-tertiary)", borderRadius: "var(--border-radius-lg)", padding: "1rem 1.25rem", display: "flex", alignItems: "flex-start", gap: "1rem" }}>
                  <div style={{ flex: 1 }}>
                    <div style={{ display: "flex", alignItems: "center", gap: "8px", marginBottom: "4px" }}>
                      <span style={{ fontWeight: "500", fontSize: "15px" }}>{o.title}</span>
                    </div>
                    <div style={{ fontSize: "13px", color: "var(--color-text-secondary)", marginBottom: "8px" }}>
                      {o.company} · <i className="ti ti-map-pin" style={{ fontSize: "13px" }} aria-hidden="true"></i> {o.location}
                    </div>
                    <div style={{ display: "flex", gap: "6px", flexWrap: "wrap" }}>
                      <span style={{ fontSize: "12px", padding: "3px 10px", borderRadius: "999px", background: c.bg, color: c.text, border: `0.5px solid ${c.border}` }}>{o.site}</span>
                      <span style={{ fontSize: "12px", padding: "3px 10px", borderRadius: "999px", background: "#EEEDFE", color: "#3C3489", border: "0.5px solid #AFA9EC" }}>{o.tag}</span>
                    </div>
                  </div>
                  <div style={{ textAlign: "right", flexShrink: 0 }}>
                    <div style={{ fontSize: "12px", color: "var(--color-text-tertiary)", marginBottom: "8px" }}>{o.date}</div>
                    <a href={o.url} style={{ fontSize: "12px", color: "#185FA5", textDecoration: "none", display: "flex", alignItems: "center", gap: "4px" }}>
                      Voir <i className="ti ti-external-link" style={{ fontSize: "13px" }} aria-hidden="true"></i>
                    </a>
                  </div>
                </div>
              );
            })}
          </div>
          <p style={{ fontSize: "12px", color: "var(--color-text-tertiary)", marginTop: "1rem" }}>Aperçu simulé — les vraies offres seront récupérées lors de l'exécution du script.</p>
        </div>
      )}

      {tab === "script" && (
        <div style={{ background: "var(--color-background-primary)", border: "0.5px solid var(--color-border-tertiary)", borderRadius: "var(--border-radius-lg)", padding: "1.25rem" }}>
          <p style={{ fontWeight: "500", margin: "0 0 0.5rem" }}>Script Python — automatisation quotidienne</p>
          <p style={{ fontSize: "13px", color: "var(--color-text-secondary)", margin: "0 0 1rem" }}>Copie ce script sur ton ordi et configure GitHub Actions ou Make.com pour le lancer chaque matin.</p>
          <pre style={{ background: "var(--color-background-secondary)", borderRadius: "var(--border-radius-md)", padding: "1rem", fontSize: "12px", overflowX: "auto", lineHeight: "1.6", color: "var(--color-text-primary)", margin: 0 }}>{`# job_newsletter.py
# Dépendances : pip install requests beautifulsoup4 yagmail schedule

import requests
from bs4 import BeautifulSoup
import yagmail
import schedule, time
from datetime import date

EMAIL_TO   = "ton@email.fr"
EMAIL_FROM = "ton.bot@gmail.com"
EMAIL_PASS = "ton_mot_de_passe_app"  # Mot de passe d'application Gmail

KEYWORDS  = ["chef de projet", "conceptrice pédagogique",
             "médiation numérique", "ingénierie pédagogique"]
LOCATION  = "Paris"

SITES = [
  {"name": "Welcome to the Jungle",
   "url": f"https://www.welcometothejungle.com/fr/jobs?refinementList[contract_type][]=CDI&query={LOCATION}"},
  {"name": "APEC",
   "url": f"https://www.apec.fr/candidat/recherche-emploi.html/emploi?motsCles={LOCATION}"},
  {"name": "Job That Makes Sense",
   "url": "https://jobs.makesense.org"},
  {"name": "Choisir le Service Public",
   "url": "https://choisirleservicepublic.gouv.fr/offres-emploi/"},
]

def scrape_offers(site):
    try:
        r = requests.get(site["url"], timeout=10,
                         headers={"User-Agent": "Mozilla/5.0"})
        soup = BeautifulSoup(r.text, "html.parser")
        offers = []
        for tag in soup.find_all(["h2","h3","a"], limit=50):
            text = tag.get_text(strip=True).lower()
            if any(kw.lower() in text for kw in KEYWORDS):
                href = tag.get("href","")
                offers.append({"title": tag.get_text(strip=True),
                                "url": href if href.startswith("http")
                                       else site["url"] + href,
                                "site": site["name"]})
        return offers[:10]
    except Exception as e:
        return [{"title": f"Erreur : {e}", "url":"", "site": site["name"]}]

def build_html(all_offers):
    today = date.today().strftime("%d/%m/%Y")
    rows = "".join(
        f"<tr><td>{o['site']}</td><td><a href='{o['url']}'>{o['title']}</a></td></tr>"
        for o in all_offers
    )
    return f"""
    <h2>Veille emploi du {today}</h2>
    <p>Offres filtrées sur : {', '.join(KEYWORDS)}</p>
    <table border='1' cellpadding='6' style='border-collapse:collapse;'>
      <tr><th>Source</th><th>Offre</th></tr>
      {rows}
    </table>
    """

def send_newsletter():
    all_offers = []
    for site in SITES:
        all_offers.extend(scrape_offers(site))
    if not all_offers:
        print("Aucune offre trouvée aujourd'hui.")
        return
    html = build_html(all_offers)
    yag = yagmail.SMTP(EMAIL_FROM, EMAIL_PASS)
    yag.send(to=EMAIL_TO,
             subject=f"🔍 Veille emploi — {date.today().strftime('%d/%m')}",
             contents=html)
    print(f"{len(all_offers)} offres envoyées.")

# Lancement quotidien à 08:00
schedule.every().day.at("08:00").do(send_newsletter)

if __name__ == "__main__":
    send_newsletter()  # Test immédiat
    while True:
        schedule.run_pending()
        time.sleep(60)
`}</pre>
          <p style={{ fontSize: "12px", color: "var(--color-text-tertiary)", marginTop: "0.75rem" }}>
            Pour l'automatisation sans laisser ton ordi allumé, utilise <strong>GitHub Actions</strong> (gratuit) avec un cron job quotidien, ou <strong>Make.com</strong> (anciennement Integromat).
          </p>
        </div>
      )}
    </div>
  );
}
