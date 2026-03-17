
<div style="text-align:center; margin: 2rem 0">
  <img src="/profile.png" width="100" style="border-radius:50%" />
  <div id="typing-text" style="font-family: monospace; font-size: 0.9rem; margin: 0.5rem 0; color: var(--darkgray); min-height: 1.5rem;"></div>
  <p>🚀 welcome to my blog! 🚀</p>
</div>

<script>
const words = ["Backend Developer", "Spring Boot", "Kotlin", "Java"];
let wi = 0, ci = 0, deleting = false;
const el = document.getElementById("typing-text");

function type() {
  const word = words[wi];
  if (!deleting) {
    el.textContent = word.slice(0, ++ci);
    if (ci === word.length) {
      deleting = true;
      setTimeout(type, 1500);
      return;
    }
  } else {
    el.textContent = word.slice(0, --ci);
    if (ci === 0) {
      deleting = false;
      wi = (wi + 1) % words.length;
    }
  }
  setTimeout(type, deleting ? 60 : 100);
}
type();
</script>

## 🪧 내 소개

It's me

## 👾 최근 개발하고 있는 것

Metrics Handling Server

## 📦 나의 프로젝트 히스토리

[Apple Care Service (Coupang)](/projects/apple-care)  
[SK T Cloud Game Pass (SKT)](/projects/skt-cloud)  
[HitaJimro AI platform project (HitaJimro)](/projects/hitajimro)  
[SMART HB Admin Platform (Chunjaetext)](/projects/smart-hb)  
[SKT Adot Project - Stock Agent, T Service (SKT)](/projects/adot)