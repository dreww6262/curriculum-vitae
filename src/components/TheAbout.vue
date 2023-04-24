<script setup lang="ts">
const quotes = [
    "3 Years of Startup Experience",
    "Cum Laude Computer Science Graduate From Virginia Tech",
    "First LGBTQIA+ President of the Aplha Pi Chapter of Zeta Psi Fraternity",
    "Alumni of FIRST Robotics"
]
</script>

<template>
    <div>
        <img alt="Profile Picture" src="@/assets/profile_pic.jpg" width="240" />
        <ul>
            <li v-for="quote in quotes">
                <h4>{{ quote }}</h4>
            </li>
        </ul>
    </div>
</template>