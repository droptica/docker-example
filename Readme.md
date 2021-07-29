# Style install (ON DEV)

    docker-compose run --rm -w /app/web/profiles/contrib/droopler/themes/custom/droopler_theme gulp npm install
    docker-compose run --rm -w /app/web/profiles/contrib/droopler/themes/custom/droopler_theme gulp gulp clean
    docker-compose run --rm -w /app/web/profiles/contrib/droopler/themes/custom/droopler_theme gulp gulp dist

    docker-compose run --rm -w /app/web/themes/custom/droopler_subtheme gulp npm install
    docker-compose run --rm -w /app/web/themes/custom/droopler_subtheme gulp gulp clean
    docker-compose run --rm -w /app/web/themes/custom/droopler_subtheme gulp gulp dist
# RUN DRUSH ON PROD

    docker-compose -f docker-compose.prod.yml exec apache drush