<template>
    <main>
        <h1>Personnages</h1>

        <div class="row">
            <div class="col-12">
                Votre selection de personnages...
            </div>
        </div>

        <div class="row">
            <div class="col-8">
                <div v-if="data">
                    <!-- Remplacer les xxx par les valeurs de l'API -->
                    <p> xxx éléments affichés sur les xxx disponible</p>
                    <p>... Liste des personnages à afficher en utilisant un composant Personnage.vue ...</p>


                    <!-- Boutons à modifier pour passer d'une page à l'autre. Désactiver le boutons si la page n'existe pas -->
                    <nav>

                        <button>Précédent</button>

                        <button>Suivant</button>
                    </nav>
                </div>
                <div v-else>
                    <p>Chargement en cours...</p>
                </div>
            </div>
            <div class="col-4 card-body card-info">
                <p>Afficher le détail d'un personnage avec une route imbriquée.</p>
                <div class="alert alert-info">
                    Veuillez sélectionner un personnage
                </div>
                <!-- Ici doit s'afficher le détail d'un personnage selectionné dans la liste à gauche -->
            </div>
        </div>
    </main>
</template>

<script setup>

const data = ref(null);
const selection = ref([]);

</script>