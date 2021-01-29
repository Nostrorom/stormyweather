<script>
    import { stores } from '@sapper/app';

    const { page } = stores();
    $: {
      if (typeof gtag !== "undefined"){
        gtag("config", "G-YFXD5VQWPW", {
          page_path: $page.path
        });
      }
    }
  </script>