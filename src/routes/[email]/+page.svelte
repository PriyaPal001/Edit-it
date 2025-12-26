<script>
    import {page} from '$app/stores';

    $: email = $page.params.email;
</script>

<div class="hero h-screen bg-base-300">
    <div class="hero-content ">
        <div class="max-w-2xl text-center">
            <h1 class=" text-5xl font-bold">{email}'s page</h1>
            <p class="py-3 max-w-md mx-auto">user descp..........</p>
            <div class="grid grid-cols-3">
                <div class="card bg-slate-700 m-4 shadow-lg shadow-blue-900">
                    <div class="card-body">
                        <div class="text-center">
                            <img src={""} alt="" class="w-32 h-32 mx-auto bg-gray-500">
                            <h2 class="text-white text-2xl font-bold">Pikachu</h2>
                            <p class="text-info">ELectric</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>