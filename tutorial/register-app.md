<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="08ad9-101">在本练习中, 你将使用 azure Active Directory 管理中心创建新的 azure AD web 应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="08ad9-101">In this exercise, you will create a new Azure AD web application registration using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="08ad9-102">打开浏览器并导航到[Azure Active Directory 管理中心](https://aad.portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="08ad9-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="08ad9-103">使用**个人帐户**(亦称: Microsoft 帐户) 或**工作或学校帐户**登录。</span><span class="sxs-lookup"><span data-stu-id="08ad9-103">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="08ad9-104">在左侧导航栏中选择 " **Azure Active Directory** ", 然后选择 "**管理**" 下的 "**应用注册 (预览)** "。</span><span class="sxs-lookup"><span data-stu-id="08ad9-104">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations (Preview)** under **Manage**.</span></span>

    ![<span data-ttu-id="08ad9-105">应用注册的屏幕截图</span><span class="sxs-lookup"><span data-stu-id="08ad9-105">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="08ad9-106">选择 "**新建注册**"。</span><span class="sxs-lookup"><span data-stu-id="08ad9-106">Select **New registration**.</span></span> <span data-ttu-id="08ad9-107">在 "**注册应用程序**" 页上, 按如下所示设置值。</span><span class="sxs-lookup"><span data-stu-id="08ad9-107">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="08ad9-108">将**名称**设置`Ruby Graph Tutorial`为。</span><span class="sxs-lookup"><span data-stu-id="08ad9-108">Set **Name** to `Ruby Graph Tutorial`.</span></span>
    - <span data-ttu-id="08ad9-109">将**支持的帐户类型**设置为**任何组织目录和个人 Microsoft 帐户中的帐户**。</span><span class="sxs-lookup"><span data-stu-id="08ad9-109">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="08ad9-110">在 "**重定向 URI**" 下, 将第一个`Web`下拉下拉箭头, 并`http://localhost:3000/auth/microsoft_graph_auth/callback`将值设置为。</span><span class="sxs-lookup"><span data-stu-id="08ad9-110">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/microsoft_graph_auth/callback`.</span></span>

    !["注册应用程序" 页的屏幕截图](./images/aad-register-an-app.png)

1. <span data-ttu-id="08ad9-112">选择 "**注册**"。</span><span class="sxs-lookup"><span data-stu-id="08ad9-112">Choose **Register**.</span></span> <span data-ttu-id="08ad9-113">在 " **Ruby Graph 教程**" 页上, 复制**应用程序 (客户端) ID**的值并保存它, 下一步将需要它。</span><span class="sxs-lookup"><span data-stu-id="08ad9-113">On the **Ruby Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![新应用注册的应用程序 ID 的屏幕截图](./images/aad-application-id.png)

1. <span data-ttu-id="08ad9-115">选择 "**管理**" 下的 "**证书 & 密码**"。</span><span class="sxs-lookup"><span data-stu-id="08ad9-115">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="08ad9-116">选择 "**新客户端密码**" 按钮。</span><span class="sxs-lookup"><span data-stu-id="08ad9-116">Select the **New client secret** button.</span></span> <span data-ttu-id="08ad9-117">在 "**说明**" 中输入一个值, 然后选择 "**过期**" 选项之一, 然后选择 "**添加**"。</span><span class="sxs-lookup"><span data-stu-id="08ad9-117">Enter a value in **Description** and select one of the options for **Expires** and choose **Add**.</span></span>

    !["添加客户端密码" 对话框的屏幕截图](./images/aad-new-client-secret.png)

1. <span data-ttu-id="08ad9-119">在离开此页面之前复制客户端密码值。</span><span class="sxs-lookup"><span data-stu-id="08ad9-119">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="08ad9-120">您将在下一步中需要它。</span><span class="sxs-lookup"><span data-stu-id="08ad9-120">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="08ad9-121">此客户端密码永远不会再次显示, 因此请务必立即复制。</span><span class="sxs-lookup"><span data-stu-id="08ad9-121">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![新添加的客户端密码的屏幕截图](./images/aad-copy-client-secret.png)