<script>
    import {supabase} from '../supabase.js';

    const logout = () => {
        console.log("log out")
        supabase.auth.signOut();
    }
</script>

<div class="my-4 flex justify-end">
    <button on:click={logout} class="shadow-sm rounded bg-gray-500 hover:bg-gray-600 text-white py-2 px-4">Log Out</button>
</div>