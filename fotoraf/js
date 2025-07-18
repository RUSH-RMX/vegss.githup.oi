const themeButtons = document.querySelectorAll('.theme-selector button');

themeButtons.forEach(btn => {
  btn.addEventListener('click', () => {
    const theme = btn.getAttribute('data-theme');
    document.body.className = ''; // önce temizle

    if(theme !== 'default') {
      document.body.classList.add(theme);
    }

    // Butonların aria-pressed güncellemesi
    themeButtons.forEach(b => b.setAttribute('aria-pressed', 'false'));
    btn.setAttribute('aria-pressed', 'true');

    // Tema bazlı arkaplan animasyonunu da kontrol edebiliriz
    // (İstersen farklı temalarda farklı animasyonlar yapılabilir)
  });
});// Görsel kutulara tıklayınca tema değiştir
document.querySelectorAll('.theme-box').forEach(box => {
  box.addEventListener('click', () => {
    const theme = box.getAttribute('data-theme');
    document.body.className = '';
    if (theme !== 'default') {
      document.body.classList.add(theme);
    }
  });
});
