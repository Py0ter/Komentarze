# Komentarze

Wystarczy prosty adblocker, który pozwala na własne filtry. W miejscu NICK wpisz nick użytkownika którego chcesz schować, najlepiej skopiowany bezpośrednio z profilu

! NICK
jeja.pl##div[id^="comment_"]:has(.nick a[href*="NICK"]) > *:not(.komentarz-autor):style(display: none !important;)

jeja.pl##div[id^="comment_"]:has(.nick a[href*="NICK"])::after:style(content: "[Zablokowany komentarz]"; display: block !important; padding: 12px 15px; background: #1f1f1f; color: #ff6666; border: 1px solid #444; margin: 5px 0; border-radius: 4px;)
