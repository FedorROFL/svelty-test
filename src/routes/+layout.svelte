<nav>
    <div class="nav-container">
      <a href="/" class="nav-logo" title="Back to Homepage">Имя Фамилия</a>
      <div class="nav-links">
        {#each nav as link}
        <a href={link.href} class="link">{link.title}</a>
        {/each}  
      </div>
    </div>
  </nav>
  <div class="container">
    <!-- Pages will be injected below -->
    <slot></slot>
  </div>
  <script>
    const nav = [
    {
      title: 'Обо мне',
      href: '/about'
    },
    {
      title: 'Блог',
      href: '/blog'
    },
    {
      title: 'Портфолио',
      href: '/project'
    },
    {
      title: 'Контакты',
      href: '/contact'
    },
    {
      title: 'temp',
      href: '/temp'
    }
  ]
</script>

  <style>
    .container {
      max-width: 1400px;
      margin: 50px auto;
    }

  </style>
  <svelte:head>
    <title>Имя Фамилия</title>
    </svelte:head>
    <div class='container'>
        <div class='info'>
            <div class='animate-background'>
                <div class='container info-container'>
                    <div class='info-text'>
                        <h1>
                            <p class='animate-text-1'>Lorem ipsum dolor sit,</p>
                            <p class='text-2'>Lorem ipsum dolor sit amet.</p>
                        </h1>
                    </div>
                    <h2 class='subtitle'>
                        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium architecto aut, cupiditate dolores
                        ducimus expedita labore nemo odio quibusdam quidem sapiente soluta.
                    </h2>
                    <div style='color:black' class='scroll-button animate-scroll' tabindex='0'>
                        <a href='/about'>Click Here</a>
                        <div class='arrow'>→</div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
    <div class='background-div'></div>
