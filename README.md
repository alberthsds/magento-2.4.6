# magento-2.4.6
Magento 2.4.6 commamd

- php bin/magento setup:install --base-url="http://dev.magento.com/" --db-host="localhost" --db-name="magento_2.4.6" --db-user="root" --db-password="" --admin-firstname="admin" --admin-lastname="admin" --admin-email="user@example.com" --admin-user="admin" --admin-password="admin@12345" --language="en_US" --currency="USD" --timezone="America/Chicago" --use-rewrites="1" --backend-frontname="admin" --search-engine=elasticsearch7 --elasticsearch-host="localhost" --elasticsearch-port=9200

- php bin/magento module:disable Magento_AdminAdobeImsTwoFactorAuth Magento_TwoFactorAuth
- php bin/magento setup:upgrade
- php bin/magento setup:di:compile
- php bin/magento cache:clean
- php bin/magento cache:flush
