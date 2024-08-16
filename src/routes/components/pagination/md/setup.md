<script lang="ts">
  import { Pagination, PaginationItem, type PaginationItemProps } from 'svelte-5-ui-lib';
  import {
    ChevronLeftOutline,
    ChevronRightOutline,
    ArrowLeftOutline,
    ArrowRightOutline
  } from 'flowbite-svelte-icons';
 
  let pages = $state([
    { name: '1', href: '/components/pagination?page=1', active: false },
    { name: '2', href: '/components/pagination?page=2', active: false },
    { name: '3', href: '/components/pagination?page=3', active: false },
    { name: '4', href: '/components/pagination?page=4', active: false },
    { name: '5', href: '/components/pagination?page=5', active: false }
  ]);
  const previous = () => {
    alert('Previous btn clicked. Make a call to your server to fetch data.');
  };
  const next = () => {
    alert('Next btn clicked. Make a call to your server to fetch data.');
  };
</script>